## HTTP+Websocket
Panasonic is planning to use Websocket to notify event for the the demo of the February Plugfest.  Based on HTTP binding, only event notification will communicate via Websocket as follows:

*Property, Action: Same as HTTP binding
*Event
  - Subscribe: POST + Open Websocket connection (return handler number)
  - Notify: Websocket notification (notify via opened Websocket)
  - Cancel subscription: DELETE + Disconnect Websocket connection
