# react-live-timezone

### **Live Coding Assignment: World Clock with Dynamic Timezone Widgets**

---

#### **Objective**
Build a **World Clock application** that allows users to:
1. Dynamically add clocks for different time zones using a dropdown.
2. Display the current time for each selected time zone.
3. (Optional) Add a personal avatar image to the top-right corner of the application.

This exercise tests your skills in:
- React component development.
- Handling dynamic state and rendering.
- Basic styling and layout using provided design guidelines.
- (Optional) File handling and user interaction for image uploads.

---

#### **Setup Instructions**

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Install Dependencies**:
   Make sure you have `Node.js` and `npm`/`yarn` installed. Install the dependencies:
   ```bash
   npm install
   ```
   or
   ```bash
   yarn install
   ```

3. **Resources**:
   - `timezones.json`: Contains an exhaustive list of time zones with GMT offsets and details.
   - `designs/`: Contains minimal design files and mockups.

4. **Start the Development Server**:
   ```bash
   npm start
   ```
   or
   ```bash
   yarn start
   ```

5. **Expected Functionality**:
   - **Dynamic Clock Widgets**:
     - Dropdown to select a time zone.
     - Add clocks dynamically for selected time zones.
     - Display the current time (auto-updating every second) for each added clock.
     - Ability to remove individual clocks.
   - **Time Zone Dropdown**:
     - Populate the dropdown using the `timezones.json` file.
   - **Responsive Design**:
     - Ensure the application works well across various screen sizes.
   - **(Optional) User Avatar**:
     - Allow users to upload an image for the avatar and display it in the top-right corner.
   - Follow the design guidelines in the `designs` folder.

---

#### **Implementation Details**

1. **World Clock Features**:
   - **Dropdown**: Use the data in `timezones.json` to populate the dropdown with `label` (e.g., "New York (GMT-5)") and `value`.
   - **Adding Widgets**:
     - Each clock should display:
       - Time zone name.
       - Current local time in that zone.
     - Use JavaScript `Date` object and GMT offset from `timezones.json` to calculate the time.
   - **Removing Widgets**:
     - Add a "Remove" button for each clock widget.
     - Removing a clock should not affect others.

2. **Avatar Feature (Optional)**:
   - Provide a button or input to upload an image.
   - Preview the image in the top-right corner of the application.
   - Ensure it doesn’t interfere with the core clock functionality.

3. **Styling**:
   - Use the design mockups in the `designs` folder as a reference.
   - Minimal and clean design is preferred.
   - Ensure the layout is responsive.

4. **Time Zone Data**:
   - Load `timezones.json` at the start of the application.
   - Example of a single time zone entry in the file:
     ```json
     {
       "label": "New York (GMT-5)",
       "city": "New York",
       "country": "United States",
       "value": "America/New_York",
       "offset": -5,
       "gmt_offset": "GMT-5"
     }
     ```

5. **Functional Requirements**:
   - Dynamically update the clocks every second.
   - Ensure clocks display time in the correct format (HH:MM:SS).

6. **Bonus Points**:
   - Implement `localStorage` or another method to persist the added clocks across browser reloads.
   - Add basic animations/transitions when adding/removing widgets.
   - Implement accessibility features (ARIA labels, keyboard navigation).

---

#### **Deliverables**

1. A functional React application fulfilling the requirements.
2. A responsive and clean UI aligned with the design mockups.
3. Code organised in reusable components.
4. Clear and meaningful comments in the code.
5. A deployed version (e.g., via GitHub Pages, Vercel, or Netlify) or instructions to run locally.

---

#### **Expected Standards**

1. **Code Quality**:
   - Readability and organisation of the code.
   - Use of reusable and modular components.

2. **Functionality**:
   - Properly working clocks with dynamic additions/removals.
   - Correct time displayed for each clock.
   - (Optional) Avatar upload functionality.

3. **Design Implementation**:
   - Adherence to the provided mockups.
   - Responsive design.

4. **Bonus Features** (Optional):
   - Data persistence.
   - Smooth animations.
   - Accessibility compliance.

---