# Multi-Tier Architecture

## Two-Tier Architecture

A two-tier architecture splits a system into two main parts: the Web/Application Tier and the Database Tier. In this lab, Nextcloud acts as the Web/Application Tier, and MariaDB acts as the Database Tier. Both containers talk to each other using Docker Compose.

## The Web/Application Tier

The Web/Application Tier handles user requests and displays the website interface. In this lab, the Nextcloud container runs the web app that users open in a browser to manage their files.

## The Database Tier

The Database Tier holds all the saved data for the application. In this lab, MariaDB saves important information for Nextcloud, such as user accounts and file details.

## Why Separate Them?

Separating the web app and database into two containers makes the system easier to manage. Each container has one job: one runs the app, and the other runs the database. This lets you update or fix each part separately while they still talk to each other.

