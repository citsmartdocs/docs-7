Title: Configuring sound notification
Description: Configuration of an audible alarm to signal to the attendant the arrival of a new ticket

# Configuring sound notification

This feature allows the configuration of an audible alarm to signal to the attendants the arrival of a new ticket in their ticket queue.

## Before getting started

* [x] Have at least one workflow defined in your CITSmart environment;
* [x] It is essential to have the minimum conditions for audio playback on your computer;

## Procedure

### Creating notification template

1. Access the functionality through the main menu System > Notificações > Notification Template;
2. Click on "New" to create the template;
3. Inform the notification data, click on "Sound Notification" and import the audio file;
4. Save the information.

### Put the "Notification" element in the flow

1. Access the main menu Workflow > Flow Design;
2. Select and edit the flow;
3. In the "Diagram" tab, click on the item "Extensions" click and hold the item "Notification" and drag to the Design area;
4. Double click on the "Notification" icon, and then on "Configuration";
5. In the "Notification Template" field, select the template for the notification;
6. Save the changes in the flow;

## What to do next

Done, from now on it will be possible to identify new tickets by the sound notification.

!!! warning "ATTENTION"

    Even if the user receives several notifications at the same time, the audible alarm will only be triggered once.

## Related

[Register notification template][1]

[Create workflow][2]


[1]:/en-us/citsmart-7/additional-features/communication-and-notification/notification/configuration/template-create.html

[2]:/en-us/citsmart-7/workflow/use/create-flow.html
