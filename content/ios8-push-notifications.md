Title: Requesting Push Notifications permissions in iOS8
Date: 2015-05-29 10:20
Tags: iphone, ios8, push notifications
Slug: ios8-push-notifications
Author: Manish Ahuja
    Requesting push notification permissions in iOS 8 is pretty simple. you first create UIUserNotificationSettings and then register the settings on UIApplication. 

```j
   
UIUserNotificationSettings* notificationSettings = [UIUserNotificationSettings settingsForTypes:(UIUserNotificationTypeAlert | UIUserNotificationTypeBadge | UIUserNotificationTypeSound) categories:nil];
[[UIApplication sharedApplication] registerUserNotificationSettings:notificationSettings];
[[UIApplication sharedApplication] registerForRemoteNotifications];
   
```