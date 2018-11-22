---
layout: page
title: Automation
use-site-title: true
bigimg: /img/homepage_light.jpeg
---

# Let's make smart light Smarter

HueHello helps you to automate your life with Philips hue smart lights. Ever wondered how to make best use of your Hue lights? Ever wanted to use lights more than on/off? 

- Yes, you can integrate your lights with your door bell
- Yes, you can setup lights to react when toast is ready
- Yes, you can blink lights when your baby wakes up
- Yes, you can turn on lights when an emergency message comes
- Yes, you can turn off lights as soon you plug your phone to charge
- Yes, there are unlimited possibilities with our broadcast mechanism

![Tasker Automation](/img/tasker/mobile_ss.webp)


With our [Tasker Plugin](/apps/tasker), you can configure events and let the lights react. Important meeting reminder? Light will turn green. Important call? Light will blink when phone rings. Forgot to put phone on charge? Light will turn red to remind. There are just unlimited possibilities. 

Our Tasker plugin works with Android Broadcast mechanism. The process is very simple.

{: .box-plain }
<br>1. First step is to create light action. What do you want when then event occurs. Blink light? Turn Off Living Room? Turn Off complete home?  Start Animated scene? (Saving the action is very easy. It is same as creating a shortcut in HueHello.)<br><br>2. You will get action id from first step. Send a broadcast with action id to trigger action.<br><br>*Easy-Peasy*

<br>

## [Broadcast](https://developer.android.com/guide/components/broadcasts)

There are 3 ways you can send a broadcast.

{: .box-bordered }
<br>1. Use an app which allows to send broadcast (There are many apps which send broadcast at events like Tasker, Automation)<br><br>Other 2 methods are for programmers OR advanced users. <br><br>2. Use adb command <br>3. Send broadcast programmatically<br>

### With other apps

When you configure other apps to send broadcast, they will need some detail. Here is the information you will need.

Package | Action | Extra
--- | --- | ---
*com.huehello.tasker* | `huehello.automation` | **id:3**


### With adb command

`adb shell am broadcast -a huehello.automation - —ei id #value`

### With Code

Send a broadcast with action and extra id (int)

```
        String action = "huehello.automation";
        Intent intent = new Intent(action);
        intent.putExtra("id", 3);
        context.sendBroadcast(intent);
```

In above examples id:3 is the action id you received from Tasker app. In your case it will be different. Please check Tasker app.

### Automation with unlimited possibilities

You can literally use lights with any event. From your door bell to toaster the possibilities are limitless. We hope you will love the Tasker HueHello and show us support.

If you have any question, feel free to [email us](mailto://huehello365@gmail.com)