#12-Hr-Clock-Logic-Circuit<
<h1>12-Hr-Clock-Logic-Circuit</h1>
<p><strong>Description of the circuit:</strong><br>
My circuit utilizes two distinct clocks: the actual clock, which holds the time incremented by the clock itself, and the alarm clock, which stores the alarm time set by the M+ and Hr+ increment buttons. The clocks are positioned at the top and bottom of the circuit, featuring similar designs. Both clocks share a display, toggled by the set alarm button placed just below the top clock (actual clock). All buttons, including clock time, AM/PM, and the alarm indicator, are located on the right side of the circuit.</p>

<p><strong>An outline of the design:</strong><br>
The gate responsible for switching between the auto clock and the manual clock employs 2 AND gates and an OR gate. Enabling the set time pin blocks the auto clock. Multiple AND gates are employed to compare the actual and alarm clocks. The comparison necessitates both true and false values (utilizing NOT gates) to ensure the passage of matching values. The switch between the actual and alarm clocks employs a concept similar to the auto clock, allowing only one set of values to be displayed by the hex digit display.</p>

<p><strong>Assumptions:</strong><br>
I assumed that incorporating a second clock would be the optimal solution, given the task's requirement to store and redisplay time after setting the alarm clock. I also assumed the need for a snooze button since the alarm should remain active until addressed, similar to real clocks. Despite the unusual request for using the same button to activate and disable the alarm, I incorporated both functionalities.</p>

<p><strong>Stage 1:</strong><br>
Design for the minutes side counter with a reset at 59 minutes.</p>

<p><strong>Stage 2:</strong><br>
Added a manual override switch to halt clock incrementation, utilizing a button (M+) for time advancement.</p>

<p><strong>Stage 3:</strong><br>
Design for the hour side counter with a reset at 12 hours.</p>

<p><strong>Stage 4:</strong><br>
Combined stages 2 and 3 for a complete 12-hour clock design.</p>

<p><strong>Stage 5:</strong><br>
Incorporated an alarm feature as a second clock holding the "alarm time." This feature allows users to switch to the alarm clock and increment it using the H+ and M+ buttons for alarm time setting. Additionally, a snooze feature was added to silence the alarm.</p>
