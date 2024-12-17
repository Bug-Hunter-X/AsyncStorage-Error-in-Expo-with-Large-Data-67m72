# AsyncStorage Error in Expo with Large Data

This repository demonstrates a bug encountered when using AsyncStorage in Expo with a large amount of data. The issue manifests as unexpected crashes or data corruption, coupled with an unhelpful error message.  The provided solution explores alternative approaches to handle substantial data within Expo.

## Bug Description
When storing large JSON objects or a considerable number of keys using AsyncStorage in Expo, the app might crash, become unresponsive, or result in data corruption.  The error message often fails to pinpoint the exact cause, making debugging challenging.

## Solution
The optimal solution depends on the nature of your data and its size. Consider these options:

* **Data partitioning:** Break down the large JSON object into smaller, manageable chunks and store them separately.
* **Alternative storage solutions:** Explore alternatives such as SQLite, MMKV, or other persistent storage solutions better suited for handling large datasets.
* **Data compression:** Before storing, compress your data to reduce its size. 

This repository illustrates both the problematic code and a possible solution using data partitioning.  Detailed instructions are provided in the comments within the code.