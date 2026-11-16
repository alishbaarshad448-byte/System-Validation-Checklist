# MediTrack SRS Validation Findings

## 1. Introduction

The purpose of this validation exercise was to evaluate the MediTrack Software Requirements Specification (SRS) and identify unclear, incomplete, ambiguous, and conflicting requirements.

Two students independently evaluated the SRS using a 19-item validation checklist. After completing their individual evaluations, both students compared their results and identified the major problems.

## 2. Comparison of Individual Runs

Both students identified the following issues:

| Checklist ID | Requirement | Problem Identified | Severity |
|---|---|---|---|
| C02 | R-07 | Multiple obligations are combined in one requirement. | Medium |
| C03, C04 | R-02 | The word "quickly" is vague and has no measurable response time. | High |
| C05 | R-03 | Double-booking prevention conditions are not defined. | Critical |
| C06 | R-04, R-05 | Appointment duration requirements contradict each other. | High |
| C07, C08 | R-06 | Reminder timing and delivery method are missing. | High |
| C09 | R-07 | Cancellation procedure is not sufficiently detailed. | Medium |
| C11 | R-12 | Normal working hours are not specified. | Medium |
| C12 | R-08 | Accessibility requirements for elderly patients are not measurable. | High |
| C13, C14 | R-09 | Medical record access permissions and security measures are missing. | Critical |
| C15 | R-10 | Emergency walk-in handling is not defined. | High |
| C16 | R-14 | Daily schedule information is not specified. | Medium |
| C17 | Missing | Clinic administrator functionality is not defined. | High |
| C18 | Missing | Data protection officer responsibilities are not defined. | High |
| C19 | Missing | Monday morning workload expectations are not specified. | High |

## 3. Major Findings

### Finding 1: Double Booking Risk

Requirement R-03 states that the system shall prevent double bookings but does not explain how overlapping appointments will be detected or prevented.

Impact: Two patients may receive the same appointment time.

### Finding 2: Contradictory Requirements

R-04 specifies that each appointment lasts 15 minutes, while R-05 allows doctors to set appointment lengths between 10 and 30 minutes.

Impact: Developers may become confused about the correct appointment duration.

### Finding 3: Performance Ambiguity

R-02 uses the word "quickly" without specifying a measurable response time.

Impact: The development team cannot properly test system performance.

### Finding 4: Missing Appointment Reminders

R-06 mentions reminders but does not specify when or how they will be delivered.

Impact: Patients may continue forgetting appointments.

### Finding 5: Medical Data Security

R-09 states that patient records must be stored securely but does not define access permissions or security controls.

Impact: Unauthorized people may access confidential medical information.

### Finding 6: Elderly Patient Accessibility

R-08 states that the system should be user-friendly for all age groups but does not specify accessibility features.

Impact: Elderly patients may face difficulties using the system.

### Finding 7: Emergency Walk-in Handling

R-10 allows receptionists to book walk-in appointments but does not explain how emergency patients should be prioritized.

Impact: Emergency patients may experience unnecessary delays.

### Finding 8: Missing Administrator Requirements

The SRS does not describe the functions available to the clinic administrator.

Impact: Important clinic management activities may not be supported.

### Finding 9: Missing Data Protection Responsibilities

The SRS does not define the responsibilities of the data protection officer.

Impact: Data privacy responsibilities may remain unclear.

### Finding 10: Monday Morning Performance

The SRS does not specify expected system performance during busy Monday mornings.

Impact: The system may become slow when many patients book appointments simultaneously.

## 4. Recommendations

1. Define clear rules for preventing double bookings.
2. Resolve the contradiction between R-04 and R-05.
3. Specify measurable system response times.
4. Define reminder timing and delivery methods.
5. Specify medical record access permissions and security controls.
6. Include accessibility requirements for elderly patients.
7. Define emergency walk-in procedures.
8. Add clinic administrator requirements.
9. Define data protection officer responsibilities.
10. Specify performance expectations during peak hours.

## 5. Conclusion

The validation exercise identified several important problems in the MediTrack SRS.

The most critical issues are double booking prevention and patient data security. The document also contains contradictory, vague, and incomplete requirements.

The SRS should be revised and validated again before the clinic signs the software development contract.
