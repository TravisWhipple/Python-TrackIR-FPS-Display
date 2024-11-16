# TrackIR Python Library
This library reads directly from TrackIR's DDL directly.
This library does not track FPS its self, but instead relies on TrackIR's API's "frame" field which is a running count of total frames produces up to this point in time.

Credit for the TrackIR python interface: https://github.com/johnflux/python_trackir

# Display FPS
This cell will generate a chart to display the FPS that TrackIR is processing at. The FPS are derived by taking the frame delta and dividing that by the time delta between polling TrackIR's "frame" data.

The "frame" data is a running total number of frames TrackIR has produced in the current session.

The blue line is a running average, where as the gray line is the raw FPS computed from the frame delta.

# Example Usage
An example of this library in action can be seen in this video: 