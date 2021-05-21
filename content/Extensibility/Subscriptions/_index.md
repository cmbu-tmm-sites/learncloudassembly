---
title: "Subscriptions"
weight: 50
---

## Extensibility subscriptions

A <strong>Subscription</strong> indicates that a subscriber is interested in being notified about an event by subscribing to an event topic and defining the criteria that triggers the notification. 

{{< img src="/Extensibility/Subscriptions/subscription-library.png" alt="Subscriptions Library" >}}

Extensibility subscriptions allow you to extend vRealize Automation [product site](https://www.vmware.com/products/vrealize-automation.html) by triggering [ABX extensibility actions](/Extensibility/Library/Actions) or vRealize Orchestrator Workflows at specific life-cycle events also known as [Event Topics](/Extensibility/Library/Event-Topics/). 

{{< img src="/Extensibility/Subscriptions/subscription-eventtopic.png" alt="Subscriptions and Event Topics" >}}

You can apply filters to your subscriptions to set boolean conditions for the specified event. 
Conditions can be created by using a javascript syntax expression.

{{< hint info >}}// Run subscription for specific user. Use when testing blocking subscriptions.<br>
<b><i>event.userName == 'username@example.com'</i></b>

// Run subscription for specific blueprint. Take the blueprint ID from blueprint page URL. 
This can be done only for provisioning related topics.<br> 
<b><i>event.data.blueprintId =='cb5c3112-3a7e-46c5-be3a-2917d0aa7741'</i></b>
{{< /hint >}}

For example, the event and workflow or action only triggers if the boolean expression is 'true'. This is helpful for scenarios where you want to control when events, actions, or workflows are triggered.

{{< img src="/Extensibility/Subscriptions/subscription-condition.png" alt="Subscriptions with Condition for execution." >}}

<strong>Action/workflow</strong>, you can select [ABX extensibility actions](/Extensibility/Library/Actions) or vRealize Orchestrator Workflows to be executd whenever there is a match for the subscription.

{{< img src="/Extensibility/Subscriptions/subscription-actionworkflow.png" alt="Subscriptions and Action / Workflow Selection" >}}

<strong>Blockable</strong>, Event Topics allow Blocking Subscriptions. Marking a subscription as Blocking will block any other subscriptions of this Blockable Event Topic and Condition, until this Action/workflow has been finished.

<strong>Timeout</strong>, is the time in minutes to wait until the Action/workflow fails. From 0 to infinite, where 0 means no timeout.
!!! Depends on the Subscription scope's "Request Timeout" of each Project (if "Any Project" option is selected as Subscription scope, you may need to manually change all Projects' "Request Timeout" if this Blocking Subscription's Timeout exceeds the Project's default "Request Timeout").

<strong>Priority</strong>, the order of execution of blocking subscription on the event topic, where 0 means highest priority, 10 means lowest (default).

<strong>Projects</strong>, define the scope where the subscription will be active. For events coming from projects not listed in the table below, this subscription will not be active. 

{{< img src="/Extensibility/Subscriptions/subscription-blockproject.png" alt="Blockable Events and other subscription settings" >}}

Subscriptions can also be versioned and compared

{{< img src="/Extensibility/Subscriptions/subscription-version.png" alt="Subscriptions and Event Topics" >}}