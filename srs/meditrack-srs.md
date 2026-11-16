
# MediTrack – Software Requirements Specification (SRS)

## Project Description

CityCare Clinic has 12 doctors, 6 receptionists, and approximately 400 patients per week.

Currently, appointments are booked using phone calls and paper diaries. This causes double bookings and long waiting times.

MediTrack is an online appointment management system designed to improve the appointment booking process.

## System Users

1. Patient
2. Doctor
3. Receptionist
4. Clinic Administrator
5. Data Protection Officer

## Manager's Main Concerns

- Double bookings must never happen.
- Patients should receive appointment reminders.
- Medical information must remain private.
- Elderly patients and emergency walk-in patients must be supported.
- The system must handle busy Monday mornings.

## Software Requirements

| ID | Requirement |
|---|---|
| R-01 | The system shall allow patients to book appointments online. |
| R-02 | The system shall respond quickly to booking requests. |
| R-03 | The system shall prevent double bookings. |
| R-04 | Each appointment shall last 15 minutes. |
| R-05 | The system shall allow doctors to set appointment length between 10 and 30 minutes. |
| R-06 | The system shall send reminders to patients before appointments. |
| R-07 | Patients may cancel appointments at any time and the system shall update the doctor's schedule and notify the receptionist. |
| R-08 | The system shall be user-friendly for all age groups. |
| R-09 | Patient records shall be stored securely. |
| R-10 | Receptionists shall be able to book appointments for walk-in patients. |
| R-11 | Patients may book up to 3 active appointments. |
| R-12 | The system shall be available during normal working hours. |
| R-13 | Overdue payments shall be handled as per clinic policy. |
| R-14 | Doctors shall be able to view their daily schedule. |
