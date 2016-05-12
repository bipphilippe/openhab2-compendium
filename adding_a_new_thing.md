# Adding a new Thing

## Inserting the device in the z-wave network
The first action is to insert the new device in the z-wave netowrk. This is to be done using the controller.

OpenHab has nothing to do at this stage. All the operation are managed from the controller itself.

## Adding the new Thing

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

To be able to finalyze configuration of the *Thing* and the linked *Items*, you have to click on "add" just below the name of the *Thing*.

You can then find the Thing in the list of Things, by clicking on *Configuration*, *Thing Configuration* in the right menu.

![](add-node-20.png)


## Configuring the Thing

You can access to the Thing configuration by clicking on *Configuration*, *Thing Configuration* in the right menu.

The Thing configuration display has 6 panels.

### Overview configuration panel

![](add-node-25.png)

This panel contains the following information:
* The label giving you the model name of the *Thing*, read-only,
* The overview, giving a description of the *Thing*, coming from the ZWave database, read-only,
* A set of controls, one per actionable *item* that has been created. You can play with the control in order to check that your device is correctly working. The name and the identifier of the *item* are read-only.

> 
The name of the item can be modified in the channels panel.

### The properties panel

![](add-node-20.png)

The properties panel presents the Label of the Thing.

You can change the label according, for example, the naming convention that we presented in the introduction.

### Configuration parameters panel

The content of this panel depends on the device model. It presents the configuration parameters of the device.



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
