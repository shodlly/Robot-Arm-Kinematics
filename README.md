

# Robot Arm Kinematics

This README provides a guide for calculating the position of the end-effector (Forward Kinematics) and determining the joint angles required to reach a target position (Inverse Kinematics) for a robot arm with three segments.

### Assumptions

- The robot arm consists of three segments with lengths \(L_1\), \(L_2\), and \(L_3\).
- Joint angles \(\theta_1\), \(\theta_2\), and \(\theta_3\) are given in degrees.
- Angles are calculated in radians where necessary.

## Forward Kinematics

**Objective:** Calculate the end-effector's position \((X_{\text{end}}, Y_{\text{end}})\) based on given joint angles \(\theta_1\), \(\theta_2\), and \(\theta_3\).

### Formulas

1. **Position of the second joint \((X_2, Y_2)\):**
 
   ![image](https://github.com/user-attachments/assets/3abd5d84-217b-420a-9c46-8817b1738dbc)


2. **Position of the third joint \((X_3, Y_3)\):**
 
   ![image](https://github.com/user-attachments/assets/792e91f8-c42f-4183-8949-df8edb1bc504)


3. **End-effector position \((X_{\text{end}}, Y_{\text{end}})\):**

  ![image](https://github.com/user-attachments/assets/01f03bd2-6946-40f8-83c6-ae0f88a3f773)


### Example Calculation

Assume:

![image](https://github.com/user-attachments/assets/12f9356d-78a7-4627-95d0-318f2deaded5)

Convert degrees to radians:

![image](https://github.com/user-attachments/assets/871b0e7e-d2b8-4d38-aa13-73844afe5738)


1. **Compute \(X_2\) and \(Y_2\):**

   ![image](https://github.com/user-attachments/assets/0ad5a85b-0572-45a7-bc83-03fe3c2579e6)


2. **Compute \(X_3\) and \(Y_3\):**

  ![image](https://github.com/user-attachments/assets/227b8bd3-857d-415c-bde1-f1c79d053f3f)


3. **Compute \(X_{\text{end}}\) and \(Y_{\text{end}}\):**

  ![image](https://github.com/user-attachments/assets/18436628-fe8a-4488-96a3-48c30892b301)


**Result:** The end-effector position is approximately \((7.70, 18.20)\).

## Inverse Kinematics

**Objective:** Determine the joint angles \(\theta_1\), \(\theta_2\), and \(\theta_3\) needed to position the end-effector at \((X_{\text{target}}, Y_{\text{target}})\).

### Formulas

1. **Compute \(\theta_3\):**

   ![image](https://github.com/user-attachments/assets/3b56ee45-a6c4-48a4-9679-0836dbc1cfeb)


2. **Compute \(\theta_2\):**

    ![image](https://github.com/user-attachments/assets/a585bc85-f0b4-4612-8005-15adc7f022ec)


4. **Compute \(\theta_1\):**

  ![image](https://github.com/user-attachments/assets/91d692eb-af86-46c5-9a20-0a4ff8445ff1)


### Example Calculation

Assume:

![image](https://github.com/user-attachments/assets/07bcd995-1b24-44cc-9880-0fbeeda825b9)


1. **Compute intermediate values:**

![image](https://github.com/user-attachments/assets/de564410-3daa-46b8-8cc0-45f530fc8656)


3. **Compute \(\theta_1\):**

  ![image](https://github.com/user-attachments/assets/43ea498b-a42d-4d0a-b549-44f3d6b209ad)


4. **Compute \(\theta_3\):**
 
  ![image](https://github.com/user-attachments/assets/fad84ab4-95fb-4e1a-a1f1-858da8e9c4cb)


**Result:** Joint angles \(\theta_1\), \(\theta_2\), and \(\theta_3\) are calculated as described.

