# datastreams
A Python module for managing data in streams.

## Usage
```python
from datastreams import DataStreamsClient, DataStream

# Create a client
client = DataStreamsClient(database='streams_db')

# Create a new data stream
stream = client.add_data_stream('my_new_stream', fields={'stream_param': 123})

# Add an entry to the stream
stream.add_entry({'wow': 'such data'})

# Get entries from stream
stream.entries

# Limit the number of entries returned
stream.get_entries(limit=10)
```