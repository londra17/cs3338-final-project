# CS3338 Final Project

## Role-Based Internal Platform for Targeted Content Delivery

This project is based on a role-based internal platform for the Santa Barbara County Public Defender’s Office. The system is designed as a SharePoint Online intranet that displays different content depending on the user’s role.

The platform uses SharePoint Framework (SPFx), React, TypeScript, SharePoint Lists, Microsoft Entra ID, Microsoft Graph API, Azure Functions, and PowerBI. The goal is to provide one centralized internal site where employees can access announcements, resources, assignments, directories, calendars, and role-specific tools.

## Project Objective

The objective of this project is to organize and document the design, requirements, workflow, testing, and deployment plan for a secure role-based intranet platform.

Instead of having multiple disconnected SharePoint pages or manually managed permissions, the system uses role-based access through Microsoft Entra ID groups. Each user sees only the tools and content that match their assigned role.

## Main Features

- Role-based navigation and content visibility
- Announcements filtered by department or role
- Staff Directory
- Expert Witness Directory
- Office Hoteling desk reservation system
- Attorney Workload Tracker
- LOP Procedure Checklist
- CDD Resource Guides
- Upcoming Events and Calendar integration
- Assignments and training workflow
- PowerBI Urgency Portal
- Content Management System for administrators

## User Roles

The platform supports the following roles:

- IT
- Compliance Officer
- HR
- Trial Supervisor
- Attorney
- CDD
- LOP
- PD-Intranet
- Everyone / Guest

Users with higher permissions, such as IT, can access more administrative tools. General users only see the content meant for their role.

## Technology Stack

- SharePoint Online
- SharePoint Framework (SPFx)
- React
- TypeScript
- Node.js 18
- pnpm
- Gulp
- Webpack
- PnP.js
- Microsoft Graph API
- Microsoft Entra ID
- Azure Functions
- PowerBI
- SharePoint Lists

## Docker Setup

This repository includes a Docker Compose file for the Docker portion of the CS3338 final project.

The actual production system is deployed through SharePoint Online as a SharePoint Framework `.sppkg` package. Because SharePoint Online, Microsoft Entra ID, Microsoft Graph API, PowerBI, and SharePoint Lists are cloud services, they are not fully containerized locally.

The Docker setup uses an NGINX container as a lightweight placeholder service to demonstrate container setup and local service execution.

## Run Docker

Make sure Docker Desktop is open.

Then run:
```bash
docker compose up
Jira Link:https://cs3338-group-8.atlassian.net/jira/core/projects/CFP/board?filter=&groupBy=status
Group 8 
