# 12-Hr-Clock-Logic-Circuit
Description of the circuit
My circuit uses two separate clocks, the actual clock that holds the time which is incremented by the clock and the alarm clock that holds the alarm time that is set by the M+ and Hr+ increment buttons. The clocks are on the top and bottom of the circuit, using very similar designs. The two clocks use the same display, which is toggled by the set alarm button. This switch occurs in just below the top clock (actual clock). All buttons are on the right side of the circuit, with the clock time, am/ pm, and alarm indicator.

An outline of the design
	The gate used to module between the auto clock and the manual clock uses 2 and gates and an or gate. By enabling the set time pin, the auto clock would be blocked.
	Many and gates were used to compare the actual and alarm clock. The comparison required both true and both false (using not gates) to ensure that all values that matched were passed through.
	My actual and alarm clock switch used a similar idea to the auto clock. Where the pin would only allow one set of values to pass through and to be displayed by the hex digit display.

Assumptions
	I assumed that a second clock would be the best solution, as the task required that the time was stored and redisplayed after the alarm clock was set.
	I assumed the alarm would need a snooze button as the alarm would stay active until action was made, like it would with a real clock. And the task requested the button used to activate the alarm would be the same as the button to disable it, which was strange in my mind. So I added both functionality.


Stage 1:
design for the minutes side counter, with a reset at 59 minutes

Stage 2:
added a manual override switch that would stop the clock from adding to the time. instead using a button (m+) to tick the clock.

Stage 3
design for the hour side counter, with a reset at 12 hours

Stage 4
combined the stage 2 and 3 for full 12 hour clock design

Stage 5:
added an alarm feature, this took form as a second clock that would hold the "alarm time" also allowing the user to switch to the alarm clock to incremnt it with the H+ and M+ buttons to set the time for the alarm. also added a snooze feature to stop the alarm from ringing.