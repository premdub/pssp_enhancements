CRUD PssP Enhancements

Further enhancements to the 'Patient Self Service Portal' with customization of the landing, login, registration, and account pages.

Changes Include:


Customized landing page that includes new logo
customized login and registration pages matching the landing page design
New user: 'Provider' with own registration page and patient editing capabilities
New redesigned account page that includes the ability to edit and delete the username and email
Account page added to heading tab
Redesign has only occurred on the landing, login, and registration pages with plans to redesign all other pages including the headings in future iterations.

Installation
Use the package manager pip to install Flask.

pip install Flask

Usage
from flask import Flask, render_template, request, redirect, url_for, flash, jsonify, abort, session, send_file
from flask_sqlalchemy import SQLAlchemy
from flask_login import LoginManager

from base64 import b64encode
import base64
from io import BytesIO  # Converts data from Database into bytes

from dotenv import load_dotenv
import os
import datetime
import uuid

from models import db, Users, Patients, Conditions_Patient, Conditions, Medications_Patient, Medications, Patients_Photos
from dashboard.blueprint import dashboard_blueprint


Requirements
Visual Studio Code
MySQLWorkbench
Azure Database for MySQL flexible server
Web Browser


Resources
Initial Database Setup: https://github.com/premdub/patient_portal

Previous Version:https://github.com/premdub/PssP

Reference Design and Setup: https://github.com/hantswilliams/HHA-504-2022

Useful Designing Tool:https://codepen.io/

Reference Templates: https://freefrontend.com/


