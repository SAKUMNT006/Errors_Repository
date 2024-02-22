Here are the steps to solve your PM2 server issue on Windows rebooting:

1. Install pm2-windows-startup: Open your command prompt and run the following command to install `pm2-windows-startup` globally:
    ```shell
    npm install -g pm2-windows-startup
    ```

2. Set up PM2 to start on boot: After installing `pm2-windows-startup`, you can set up PM2 to start on boot by running the following command in your command prompt:
    ```shell
    pm2-startup install
    ```

3. Start Your Application: Start your application with PM2 using the following command. Replace `<your-app.js>` with your actual application file.
    ```shell
    pm2 start eco.config.js
    ```

4. Save the Current State: After your application is running, save the current state with the following command. This will make PM2 remember the current running applications even after a reboot.
    ```shell
    pm2 save
    ```

5. Check Logs: You can check the logs of your application using the following command. This will show you the output of your application and any error messages if it crashes.
    ```shell
    pm2 logs
    ```

