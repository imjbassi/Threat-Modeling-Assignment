# Threat Modeling Assignment

This repository contains the work for a comprehensive threat modeling assignment utilizing **OWASP Threat Dragon**. The assignment demonstrates the capability to represent a web application using data flow diagrams and analyzes threats associated with application components using the **STRIDE** threat assessment model.

---

## Application Overview

The modeled web application performs the following functionalities:

- Presents a login page (username and password).
- Authenticates users using an open-source authentication component connected to a database.
- Retrieves and displays a "message-of-the-day" upon successful authentication.
- Allows users to submit comments on the message, which are stored in the database.

---

## Threat Modeling Process

The modeling was performed using **OWASP Threat Dragon**, following these steps:

- Authenticated through GitHub.
- Created a new threat model titled "Initial Threat Model".
- Generated a detailed data flow diagram (DFD), clearly marking boundaries and data flows among the user, web application, authentication component, and database.

---

## Identified Threats (STRIDE Model)

The following threats were identified and analyzed using the STRIDE threat model:

1. **Spoofing (Authentication)** - An attacker could impersonate a legitimate user, gaining unauthorized access.
2. **Tampering** - Unauthorized modification of data, such as comments or the message-of-the-day.
3. **Repudiation** - Users could deny performing an action, leading to accountability issues.
4. **Information Disclosure** - Sensitive information (user credentials, comments) could be exposed unintentionally.
5. **Elevation of Privilege** - An attacker might exploit the open-source authentication component, escalating privileges within the application.

---

## Impact of Open-Source Authentication Component

Using an open-source authentication component introduces potential security risks such as unknown vulnerabilities or unpatched exploits, significantly affecting system integrity and user trust. Regular updates, careful vetting, and monitoring of security advisories become critical.

---

## Recommended Mitigation Strategy

For the identified threat of **Elevation of Privilege**, the recommended action is to **Mitigate**. This involves:
- Regularly updating and patching the open-source authentication component.
- Implementing strict access control and monitoring logs for suspicious activities.
- Conducting periodic security assessments and penetration tests.

---

## About

This repository provides insights and practical examples on implementing threat modeling using industry-standard tools and methodologies.

---


