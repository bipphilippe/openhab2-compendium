# Configuring a Thing
You can access to the Thing configuration by clicking on *Configuration*, *Thing Configuration* in the right menu.

The Thing configuration display has 6 panels.

## Overview configuration panel

![](add-node-25.png)

This panel contains the following information:
* The label giving you the model name of the *Thing*, read-only,
* The overview, giving a description of the *Thing*, coming from the ZWave database, read-only,
* A set of controls, one per actionable *item* that has been created. You can play with the control in order to check that your device is correctly working. The name and the identifier of the *item* are read-only.

> 
The name of the item can be modified in the channels panel.

## The properties panel

![](add-node-20.png)

The properties panel presents the Label of the Thing.

You can change the label according, for example, the naming convention that we presented in the introduction.

## Configuration parameters panel

This panel presents the configuration parameters of the device

The content of this panel depends on the device model.

The use of these parameters are described in the user's manual of the device itself.

![](add-node-26.png)

## Association group panel

<<<< TO BE COMPLETED >>>>

## Device configuration panel

<<<< TO BE COMPLETED >>>>


## Channels panel

This panel is the key panel to configure the *Items*, as the channels are the link between *Things* and *Items*.

![](add-node-35.png)

Basically, HABmin will create one *Item* per channel.

Each channel follows the same following structure:

![](thing-channels-1.png)

Five buttons allow different actions:

![](thing-channels-2.png)
HABmin 2 creates and link automatically the needed *items* when a *thing* is created, so creating, deleting and linking action are not often used.

To personnalise item information, the *edit linked data* button opens the following window:

![](add-node-40.png)

This window allows to :
* 
change the label, making it more informative;
modify the item type if needed;
modify the category if needed.












