# CSA02
C Programming
Tasks 1–10 | Grama Jyothi Rural Electricity Co-operative
Common assumptions used throughout Tasks 1–10
• The meter is a 16-bit unsigned register, range 0–65,535, and can roll over once between two readings. The consumption calculation is modulo 65,536.
• The tariff is: first 100 units free; units 101–200 at 225 paise/unit; units above 200 at 450 paise/unit. Fixed charge = 5,000 paise
• All charges are represented as whole paise. No tax, subsidy, arrears or category-specific tariff is included because none is specified. Household category is stored for future tariff extension.
• For the complete validation program, a lower current reading is treated as a plausible rollover only when previous ≥ 60,000 and current ≤ 5,535. This is an explicit operational assumption to reject ordinary invalid decreases; the utility must tune it to its reading interval and meter policy.
• Maximum one-interval consumption is 65,535 units. District-scale total means the sum of bills for 800,000 households.




