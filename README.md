# Expo: Constants.deviceName Unavailable in Background Tasks

This repository demonstrates a common issue when using Expo's `Constants.deviceName` and similar APIs within background tasks or service workers. The `Constants.deviceName` API is intended for use within the main application context and might not be available in detached contexts.

This repo shows how to handle this situation by modifying code execution to avoid using `Constants.deviceName` outside the main application thread or presetting environment variables during background task initialization.