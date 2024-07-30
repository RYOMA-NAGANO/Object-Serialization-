# Object-Serialization
What is Serialization?

Serialization is the process of converting an object into an ordered byte stream for transmission over a network or storage in a local file. The core function is to preserve and reconstruct the state of objects. Desialization: The client obtains a serialized object byte stream from a file or network, and reconstructs the object through deserialization based on the object state and description information stored in the byte stream.

What is Data Persistence?

The process of data persistence is to write data to a persistent device (such as a hard drive). After the system restarts, these data will not be lost and can still be read from persistent devices.

We will earning how to store an object consistently, namely Data Persistence. Using python and by ways of serialization and deserialization to achieve goals. Separating tasks into steps:

1:  Define an object Object whose class object content format is singleton mode

2:  Write different functions for serialization, deserialization, encrypting and decrypting files, storing files, and loading files.

3:  Simulate a scene, store the objects, close the program, restart and load, requiring consistency between the stored and loaded objects

After comparing two serialization methods(dill,pickle), we have found out that dill is extended pickle package such that str in python will be the same but their time usage will be different, dill takes longer than pickle.

