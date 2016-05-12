# Adding a new Thing

## Inserting the device in the z-wave network
The first action is to insert the new device in the z-wave netowrk. This is to be done using the controller.

OpenHab has nothing to do at this stage. All the operation are managed from the controller itself.

## Setting up the new Thing

A fex seconds after your device has been inserted inside the network using the controler, a new Thing appears in the inbox.

As you can see in the following picture, a small green label with the number of new things appears at the top right of the habmin 2 screen.

![](add-node-10.png)

If you click on it, the inbox pops up with the list of the newly detected Things.

![](add-node-15.png)

As you can see in the previous screenshot, Habmin is able to find out the model of the device that the Things represents. This allows Habmin to automatically setup the corresponding Items.

The "Z-Wave Node 2" mention gives the OpenHab internal number of the zwave node, in our case 2.


> Habmin is using an internal database to fetch configuration data corresponding to the device.


> If this device is not in the database,then no device name nor model will be displayed but a code identifying the device.

> ![](zwave-node-badnode.png)

> In this example, the Thing "Z-wave Node 3" has not been found in the ZWave database and the Thing "Z-wave Node 4"  has been successfully identified.
> 
> The section *The ZWave Database* details more the database and how you can send information about a new device.





![](add-node-20.png)

![](add-node-25.png)

![](add-node-30.png)

![](add-node-35.png)

![](add-node-40.png)

![](add-node-45.png)

![](add-node-50.png)

![](add-node-55.png)

![](add-node-60.png)

![](add-node-65.png)

![](add-node-70.png)

![](tool-network.png)
