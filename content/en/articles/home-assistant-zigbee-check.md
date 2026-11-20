---
title: "Home Assistant: first checks after a Zigbee2MQTT outage"
description: "A troubleshooting checklist for Zigbee2MQTT without resetting your entire Zigbee network."
date: 2026-11-20
draft: true
translationKey: zigbee2mqtt-first-checks
slug: "home-assistant-zigbee2mqtt-troubleshooting"
categories: ["Smart Home"]
---
> **Editorial draft:** test in a lab before publishing.

## 1. Observe before changing anything

Identify whether the issue affects a single device or the entire network. Read Zigbee2MQTT logs and check the MQTT broker status.

## 2. Check the coordinator

Ensure the Zigbee adapter is detected, its serial path hasn't changed and no other service is locking the device.

## 3. Avoid destructive resets

Back up your configuration before making changes. Do not delete the Zigbee database or re-pair every device without identifying the cause.

## 4. Verify the fix

Check device reconnections, MQTT messages and Home Assistant device status. Document the root cause.
