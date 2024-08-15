# AID ME

## API URL (backend)

```
https://aid-me-backend.onrender.com
```

## URL Of The Site (frontend)

```
https://aid-me-frontend.onrender.com
```

## Introduction

In the aftermath of disasters, whether natural or human-made, providing aid to affected communities poses significant challenges. Non-Governmental Organizations (NGOs) often struggle with logistical complexities, making it difficult to deliver necessary resources and manage relief efforts efficiently. Aid-Me aims to alleviate these challenges by offering a centralized platform designed to streamline the processes of planning, executing, and managing aid operations.

## Project Objective

The primary objective of Aid-Me is to reduce the burden on NGOs by providing a comprehensive tool that facilitates the creation, development, deployment, and management of disaster relief plans. This platform will help organizations efficiently manage camps, track individuals and families, and oversee donations, ensuring a more effective response to disaster situations.

## Target Users

The main users of the Aid-Me application will include:
Members of NGOs responsible for managing disaster relief efforts
Government agencies and international bodies providing aid and donations
Research centers and academic institutions conducting studies on disaster management and humanitarian aid

## Key Features

- User Management: Secure sign-up and login for authorized personnel.
- Data Management: Full CRUD (Create, Read, Update, Delete) operations for managing information about individuals, families, disaster sites, and donations.
- Database Structure: Separate tables for individuals, families, disaster sites, and donations, with relationships mapped accordingly to facilitate efficient data management.
- Data Security: Robust measures to protect sensitive information both at rest and in transit.
- Filtering and Sorting: Advanced features to filter and sort data based on various criteria, aiding decision-making processes.

## Technical Approach

- Technologies Used: The application will be developed using Node.js for the back-end and React.js for the front-end, among other supporting technologies, to create a full-stack web application. Future plans include developing a mobile app version.
- Database Design: The database will include tables for individuals, families, disaster sites, and donations, with necessary relationships to enable efficient data management.

## Expected Benefits

Efficiency: Streamlined operations for NGOs and aid organizations, reducing the complexity of managing disaster relief efforts.
Transparency: Clear tracking of donations and resource allocation, ensuring accountability.
Data Security: Enhanced protection of sensitive information, complying with data protection regulations.
Scalability: Potential for future expansion, including the development of a mobile app version to further enhance accessibility and usability.

## Conclusion

Aid-Me aims to revolutionize the management of disaster relief efforts by providing a centralized, user-friendly platform for NGOs and related organizations. By leveraging modern technologies and focusing on user needs, Aid-Me will significantly enhance the efficiency and effectiveness of humanitarian aid, ensuring that help reaches those in need more quickly and effectively.

## Different Routes
- `/camps/[id]`
- `/people`
- `/families/[id]`
- `/families/[id]/people`
- `/families/[fID]/people/[pID]`
- `/families/household`
- `/families/[fID]/donations`
- `/families/[fID]/donations/[dID]`
- `/donations/[id]`
- `/auth/token`

## Token
If using an API client, generate a `token` by going to `auth/token` and passing `{"username":"admin", "password": "admin"}` to the body. Add the `token` in the header as `authorization: [GENERATED_TOKEN]`. If using the site, `login` with the same credentials.
