---
A:
  - Text: "Individual with ≥T6 SCI & Symptoms of AD"
  - BoxPosition: [81, 8]
  - BoxDimensions: [245, 48]
  - Next:
    - A2: Continuous
A2:
  - Text: "Check BP: is sBP ≥20 mmHg (adult) or ≥15 mmHg (child) from baseline?"
  - BoxPosition: [60, 68]
  - BoxDimensions: [291, 45]
  - Next:
    - C1: No
    - B1: Yes
B1:
  - Text: "Sit person upright, lower legs, and loosen tight clothing, compression stockings/abdominal binder."
  - BoxPosition: [168, 141]
  - BoxDimensions: [222, 104]
  - Next:
    - B2: Continuous
B2:
  - Text: "Monitor BP q2-5min. Is systolic BP improving/resolved?"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - C2: No
    - B3: Yes
B3:
  - Text: "Monitor BP every 2-5min if resolving, instruct individual to monitor BP for 2 hours post-AD."
  - BoxPosition: [265, 262]
  - BoxDimensions: [126, 147]
  - Next:
    - N1: Continuous
C1:
  - Text: "Cause of symptoms not identified - refer to appropriate consultant"
  - BoxPosition: [3, 141]
  - BoxDimensions: [150, 122]
  - Next:
    - C2: Continuous
C2:
  - Text: "Does this person have an indwelling urethral or suprapubic catheter?"
  - BoxPosition: [3, 205]
  - BoxDimensions: [150, 58]
  - Next:
    - E1: No
    - D1: Yes

D1:
  - Text: "Unkink tubing, empty drainage bag if present. Is bladder draining?"
  - BoxPosition: [3, 285]
  - BoxDimensions: [123, 60]
  - Next:
    - D2: Continuous
D2:
  - Text: "Monitor BP q2-5min. Is BP improving?"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - F1: No
    - J1: Yes
E1:
  - Text: "Instill 2% lidocaine into urethra (if available); wait 4-6 minutes to catheterize bladder"
  - BoxPosition: [135, 285]
  - BoxDimensions: [124, 60]
  - Next:
    - E2: Continuous
E2:
  - Text: "Did urine drain from the bladder?"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - I2: No
    - G1: Yes
F1:
  - Text: "Check for catheter blockage, gently irrigate catheter 10-15cc for adult (5-10cc for child). Is Catheter blocked?"
  - BoxPosition: [3, 368]
  - BoxDimensions: [123, 60]
  - Next:
    - I1: No
    - H1: Yes
G1:
  - Text: "Monitor BP while bladder is draining. Is BP improving/resolved?"
  - BoxPosition: [137, 370]
  - BoxDimensions: [119, 39]
  - Next:
    - I2: No
    - B3: Yes
H1:
  - Text: "Remove catheter and instill 2% lidocaine jelly into the urethra (wait 4-6 minutes), insert new catheter."
  - BoxPosition: [135, 285]
  - BoxDimensions: [124, 60]
  - Next:
    - H2: Continuous
H2:
  - Text: "If unable to remove or insert catheter, consult urologist or ED, give pharmacological treatment to urologist or ED"
  - PopupUrl: "algorithms/popups/pharmacology-steps.md"
  - PopupTitle: "Cutoffs ⤴"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - H3: Continuous
H3:
  - Text: "Monitor BP. Is BP improving?"
  - BoxPosition: [137, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - I2: No
    - J1: Yes
I1:
  - Text: "Patient to monitor BP 2 hours post-AD for hyper/hypotension"
  - BoxPosition: [76, 432]
  - BoxDimensions: [180, 130]
  - Next:
    - I2: Continuous
I2:
  - Text: "Consider Fecal Impaction"
  - BoxPosition: [76, 432]
  - BoxDimensions: [180, 130]
  - Next:
    - I3: Continuous
I3:
  - Text: "Note: Prior to laying down to check rectum, give pharmacological agent if sBP > 150 mmHg"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - I4: Continuous
    - M1:
      - Text: "Pharmacology Steps ⤴"
      - Style: "Neutral"
      - Type: "Custom"
I4:
  - Text: "Is rectum full?"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - L1: No
    - K1: Yes
J1:
  - Text: "Monitor BP post-AD for 2 hours - recurrent hyper/hypotension?"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - K6: No
    - K5: Yes
K1:
  - Text: "Instill lidocaine jelly into rectum and wait 4-6 minutes before checking rectum"
  - BoxPosition: [76, 585]
  - BoxDimensions: [180, 232]
  - Next:
    - K2: Continuous
K2:
  - Text: "If rectum full, begin manual disimpaction"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - K3: Continuous
K3:
  - Text: "Monitor BP post-AD for 2 hours during disimpaction - recurrent hyper/hypotension?"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - K4a: Continuous
K4a:
  - Text: "If BP elevates during disimpaction, stop, give pharmacological intervention and wait 20 minutes. Send to ED if elevated BP persists"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
      - K5:
          - Text: "Ongoing AD"
          - Style: "Red"
          - Type: "Custom"
      - K4b:
          - Text: "Success"
          - Style: "Green"
          - Type: "Green"
K4b:
  - Text: "Disimpaction successful. Is BP improving or resolved?"
  - BoxPosition: [266, 706]
  - BoxDimensions: [125, 56]
  - Next:
    - K5: No
    - N1: Yes
K5:
  - Text: "If no obvious trigger & BP remains elevated, reoccurs, or unable to manage hypotension, send to ER or admit for evaluation & management of BP/AD."
  - BoxPosition: [76, 705]
  - BoxDimensions: [180, 112]
  - Next:
    - K6: Continuous
K6:
  - Text: "Post-AD Episode. Document episode and treatment, educate patient, evaluate for preventative measures/medications"
  - BoxPosition: [76, 705]
  - BoxDimensions: [0, 0]
L1:
  - Text: "Check for other obvious triggers"
  - BoxPosition: [2, 583]
  - BoxDimensions: [67, 68]
  - Next:
    - K5:
      - Text: "No triggers found"
      - Style: "Red"
      - Type: "Custom"
M1:
  - Text: "Give pharmacologic treatment if elevated sBP remains"
  - PopupUrl: "algorithms/popups/bp-cutoffs.md"
  - PopupTitle: "Cutoffs ⤴"
  - BoxPosition: [273, 415]
  - BoxDimensions: [118, 50]
  - Next:
    - M2: Continuous
M2:
  - Text: "After pharmacological treatment, recheck BP. Is BP still above cutoff?"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - K1: No
    - O1: Yes
N1:
  - Text: "Monitor BP post-AD for recurrent hyper/hypotension"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - K6:
        - Text: "Post-AD Episode"
        - Style: "Green"
        - Type: "Custom"
    - K5:
        - Text: "Recurrence"
        - Style: "Red"
        - Type: "Custom"
O1:
  - Text: "Give additional pharmacological treatment"
  - BoxPosition: [273, 511]
  - BoxDimensions: [118, 114]
  - Next:
    - O2: Continuous
O2:
  - Text: "Monitor BP q2-5 min until below cutoff (i.e. <150 mmHg in adults). Still above cutoff?"
  - PopupUrl: "algorithms/popups/bp-cutoffs.md"
  - PopupTitle: "Cutoffs ⤴"
  - BoxPosition: [0, 0]
  - BoxDimensions: [0, 0]
  - Next:
    - K1: No
    - O3: Yes
O3:
  - Text: "Send to ED/hospital admission"
  - BoxPosition: [246, 641]
  - BoxDimensions: [125, 47]
---
