Hey guys, today we gonna make a presentation on our work ble.
Here is the index of content.
First, I gonna introduce you about the setup, scan as well as the connection of the ble devices.
Then my colleges will continue on how to read data from the ble devices as well as write data to the ble devices.

As for the setup.
First, we have to add some permissions and features into the manifest file which is included in the Android Studio project.
For example, we have to add these two bluetooth permissions so that the app can access the bluetooth service.
And as for Android 6.0, we have to add the location permissions and turn on the GPS service manually.
Once we run the app, it will automatically check if ble is supported on the device. 
If it is yes, it will initialize the bluetooth adapter and be ready to scan the bluetooth devices.

As for the scanning, StartLeScan is the key function. Since scanning a energy-consuming operation.
The postDelay function will be used to stop scanning after a pre-defined scan period.
And, the LeScanCallback is a callback function which is used to deliver LE scan results.

Then it comes to the connecting.
The class BluetoothGatt provides functions to enable communication between bluetooth devices.
And, the connectGatt is a function in the class BluetoothDevice.
It will return an instance of bluetoothGatt to build the connection.
GattCallBack as a callback function, is used to transfer the connection status and result.
For example, some functions could be defined to react when services are found, characteristics are read or written.

Here is the device scan activity where some discovered ble devices are listed.
Once the certain device is clicked. The name and mac address of the device will be transferred to the next activicy.
So, my colleges will introduce you about how to read and write data through ble devices in detail. 



