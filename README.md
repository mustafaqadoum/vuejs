### **Hiring Task #004**: Frontend Developer (Vue.js + SIP.js) - **XCalls Project**

---

**Position**: Frontend Developer  
**Technology Stack**: **Vue.js**, **SIP.js**, **VoIP**

---

### **Objective**:
This task is designed to evaluate your skills in developing an interactive frontend application using **Vue.js**, **SIP.js**, and other VoIP technologies. The aim is to assess your ability to build a feature-rich call interface that handles both outbound and inbound VoIP calls, displays call summaries, and logs call data. Furthermore, you will ensure proper integration with the provided **SIP server** and verify the accuracy of your implementation through pre-testing.

---

### **Task Overview**:

You are expected to implement the following functionalities in a **Vue.js** application utilizing **SIP.js**:

1. **Outbound Call Handling**:  
   - Implement a form where users can input a phone number and initiate an outbound VoIP call using **SIP.js**. You are to use the provided **SIP account credentials** (details below) to connect to the server and place the call.
   - Once a call is initiated, the application should provide real-time updates, including the call's status (ringing, in progress, ended) and any relevant call controls, such as ending the call.

2. **Inbound Call Handling**:  
   - Implement functionality to receive incoming calls using **SIP.js**. When a call arrives for the configured SIP account, display a notification with options to **answer** or **reject** the call. If the user answers, the call should be connected, and the interface should show that the call is active.
   - The application should allow users to reject calls, and this status should be appropriately handled in the UI.

3. **Call Summary**:  
   - Once the call has ended, generate and display a call summary that includes:
     - Call start time
     - Call end time
     - Total call duration (in seconds or minutes)
   - This information should be presented to the user in a simple yet clear format to give them a concise overview of the call.

4. **Call Logging**:  
   - Maintain a **call log** for all calls made or received during the session. Each call entry should include the following:
     - Call start time
     - Call duration
     - Call status (answered, missed, or rejected)
   - The log should be accessible during the session and provide a full overview of all recent interactions.

---

### **SIP Account Details**:

You will use the following **SIP account credentials** for this task. Ensure that the application is fully integrated with these details:

- **Username**: `101`
- **Password**: `severalleddepend8912@@`
- **SIP Domain**: `sip.xtrevo.com`
- **WebSocket URL**: `wss://sip.xtrevo.com:8443/asterisk-wss`

These credentials will allow you to connect to the **Asterisk SIP server** hosted at `sip.xtrevo.com` via WebSocket. You will use this configuration to handle both outbound and inbound calls.

---

### **Pre-Implementation Testing**:

Before you begin coding, you are required to validate the provided SIP account credentials by testing them on the **Innovate Asterisk Web Phone**. This is essential to ensure that the SIP server is properly configured and that the provided credentials work as expected.

#### **Testing Steps**:
1. Access the **Innovate Asterisk Web Phone** here:  
   [https://www.innovateasterisk.com/phone/](https://www.innovateasterisk.com/phone/)
   
2. Enter the provided **SIP account credentials**:
   - **Username**: `101`
   - **Password**: `severalleddepend8912@@`
   - **SIP Domain**: `sip.xtrevo.com`
   - **WebSocket URL**: `wss://sip.xtrevo.com:8443/asterisk-wss`

3. Verify that you can successfully make and receive calls using the web phone. Once the credentials have been validated, proceed with the implementation by integrating them into your Vue.js application.

---

### **Detailed Task Requirements**:

1. **Frontend Development Using Vue.js**:  
   - Your implementation must use **Vue.js** to create a modular and scalable frontend application. Focus on creating components for each functionality, including call controls, call status display, and call logging.
   - The UI should be intuitive, responsive, and visually clean, providing users with a seamless experience when making or receiving calls.

2. **SIP.js Integration for VoIP Calls**:  
   - Integrate **SIP.js** to manage the VoIP call functionality. The application should be capable of:
     - Making outbound calls using the SIP credentials.
     - Receiving and answering incoming calls.
     - Properly managing call states (initiated, ringing, active, ended).
   - Ensure that SIP.js events are handled appropriately and that the call interface updates dynamically as calls progress.

3. **Handling Call Events**:  
   - The application must correctly handle all major call events:
     - **Initiating a call**: When a user dials a number, the app should show the call status (ringing, connecting, or in progress).
     - **Receiving a call**: When an incoming call is detected, the user should be presented with an option to either accept or reject the call.
     - **Ending a call**: Ensure that the UI updates accordingly when a call is terminated.
   - You should implement error handling for failed or missed calls, ensuring that users are notified of any issues that occur during the process.

4. **Call Summary and Logging**:  
   - After each call, a **call summary** should be displayed, providing details about the call, including start and end times and total duration.
   - Implement a **call log** that tracks all calls (both inbound and outbound) during the session. The log should provide an overview of:
     - When the call was made or received.
     - How long the call lasted.
     - Whether the call was answered, missed, or rejected.

5. **UI/UX Design**:  
   - The interface must be user-friendly, clear, and accessible. Ensure that call statuses (active, ended, rejected) are displayed prominently so that users can quickly assess the state of the call.
   - Provide appropriate visual cues for incoming calls (e.g., a notification or alert), and ensure that the call controls are intuitive (e.g., buttons for answering, rejecting, and ending calls).

---

### **Evaluation Criteria**:

Your submission will be evaluated based on the following criteria:

1. **Code Quality**:
   - Efficient use of Vue.js components.
   - Clean, maintainable, and well-documented code.
   - Handling state and events correctly with Vue.js and SIP.js.

2. **SIP.js and VoIP Expertise**:
   - Successful integration of SIP.js for VoIP call handling.
   - Ability to manage different call states and transitions smoothly.
   - Proper handling of SIP events such as call initiation, reception, and termination.

3. **UI/UX Design**:
   - The user interface should be intuitive and provide clear feedback for all actions (e.g., making, receiving, and ending calls).
   - A well-organized display for call summaries and logs.

4. **Pre-Implementation Testing**:
   - The SIP account credentials must be validated using the **Innovate Asterisk Web Phone** before being integrated into the Vue.js application.
   - You must confirm that the SIP server works as expected with the provided account.

5. **Call Summary and Logging**:
   - Detailed and accurate logging of call data.
   - Displaying clear and informative call summaries after each interaction.

---

### **Additional Information**:

- **SIP User 101**: Use the following test credentials for your implementation:
  - **Username**: `101`
  - **Password**: `severalleddepend8912@@`
  - **SIP Server**: `wss://sip.xtrevo.com:8443/asterisk-wss`

- **Testing**: You are required to test the call-making and receiving functionality with **SIP user 101** on the provided SIP server. Ensure proper configuration and handling of the SIP connection.

- **Resources**:
   - **SIP.js Documentation**: [https://sipjs.com/](https://sipjs.com/)
   - **Vue.js Documentation**: [https://vuejs.org/](https://vuejs.org/)

---

### **Footer**:

This task is related to **Hiring Task #004**.

For more information, feel free to reach out to us:

- **Email**: admin@netronsolutions.com  
- **Phone**: +971 50 245 0637

This task was written by **Mustafa Qadoum** for **NetronSolutions**.

---

**About NetronSolutions**:

NetronSolutions is a technology-driven company specializing in custom software development, communication systems, and VoIP solutions. We pride ourselves on delivering innovative, high-quality solutions to our clients across various industries. For more information, visit [www.netronsolutions.com](https://www.netronsolutions.com).

Good luck! This task is designed to test both your frontend development skills using Vue.js and your understanding of real-time communication protocols like **SIP** and VoIP systems. Be sure to validate the SIP credentials using the **Innovate Asterisk Web Phone** before proceeding with your implementation to ensure everything is configured correctly.
