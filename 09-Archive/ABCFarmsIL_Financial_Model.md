# ABCFarmsIL Financial Model Structure

Below is the structure and formulas for an Excel financial model for ABCFarmsIL. This can be implemented in Excel by following this structure.

## Worksheet 1: Dashboard

### Summary Metrics
| Metric | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|--------|--------|--------|--------|--------|--------|
| Revenue | =SUM('Revenue Projections'!B14) | =SUM('Revenue Projections'!C14) | =SUM('Revenue Projections'!D14) | =SUM('Revenue Projections'!E14) | =SUM('Revenue Projections'!F14) |
| COGS | =SUM('COGS'!B12) | =SUM('COGS'!C12) | =SUM('COGS'!D12) | =SUM('COGS'!E12) | =SUM('COGS'!F12) |
| Gross Profit | =B4-B5 | =C4-C5 | =D4-D5 | =E4-E5 | =F4-F5 |
| Gross Margin % | =B6/B4 | =C6/C4 | =D6/D4 | =E6/E4 | =F6/F4 |
| Operating Expenses | =SUM('OpEx'!B20) | =SUM('OpEx'!C20) | =SUM('OpEx'!D20) | =SUM('OpEx'!E20) | =SUM('OpEx'!F20) |
| EBITDA | =B6-B9 | =C6-C9 | =D6-D9 | =E6-E9 | =F6-F9 |
| EBITDA Margin % | =B10/B4 | =C10/C4 | =D10/D4 | =E10/E4 | =F10/F4 |
| Net Income | =B10*0.8 | =C10*0.8 | =D10*0.8 | =E10*0.8 | =F10*0.8 |
| Net Margin % | =B12/B4 | =C12/C4 | =D12/D4 | =E12/E4 | =F12/F4 |

### Key Performance Indicators
| KPI | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|-----|--------|--------|--------|--------|--------|
| Number of Chef Clients | ='Revenue Projections'!B4 | ='Revenue Projections'!C4 | ='Revenue Projections'!D4 | ='Revenue Projections'!E4 | ='Revenue Projections'!F4 |
| Average Trays per Week | ='Revenue Projections'!B5 | ='Revenue Projections'!C5 | ='Revenue Projections'!D5 | ='Revenue Projections'!E5 | ='Revenue Projections'!F5 |
| Average Tray Price | ='Revenue Projections'!B6 | ='Revenue Projections'!C6 | ='Revenue Projections'!D6 | ='Revenue Projections'!E6 | ='Revenue Projections'!F6 |
| Total Trays per Year | ='Revenue Projections'!B7 | ='Revenue Projections'!C7 | ='Revenue Projections'!D7 | ='Revenue Projections'!E7 | ='Revenue Projections'!F7 |
| COGS per Tray | ='Unit Economics'!B5 | ='Unit Economics'!B5 | ='Unit Economics'!B5 | ='Unit Economics'!B5 | ='Unit Economics'!B5 |
| Profit per Tray | ='Unit Economics'!B7 | ='Unit Economics'!B7 | ='Unit Economics'!B7 | ='Unit Economics'!B7 | ='Unit Economics'!B7 |
| Break-even Trays/Month | ='Break-even Analysis'!B10 | ='Break-even Analysis'!C10 | ='Break-even Analysis'!D10 | ='Break-even Analysis'!E10 | ='Break-even Analysis'!F10 |

### Charts
1. Revenue Growth Chart (Bar Chart)
2. Gross Margin & EBITDA Margin (Line Chart)
3. Chef Client Growth (Line Chart)
4. Monthly Cash Flow (Line Chart)

## Worksheet 2: Revenue Projections

### Chef Client Growth
| Period | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|--------|--------|--------|--------|--------|--------|
| Number of Chef Clients | 7 | 20 | 40 | 60 | 90 |
| Average Trays per Week per Chef | 4 | 4.5 | 5 | 5.5 | 6 |
| Average Tray Price | $30 | $32 | $34 | $35 | $35 |
| Total Trays per Year | =B4*B5*52 | =C4*C5*52 | =D4*D5*52 | =E4*E5*52 | =F4*F5*52 |
| Revenue from Microgreens | =B7*B6 | =C7*C6 | =D7*D6 | =E7*E6 | =F7*F6 |

### Additional Revenue Streams
| Revenue Stream | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|----------------|--------|--------|--------|--------|--------|
| Heritage Eggs | $0 | $48,000 | $90,000 | $144,000 | $216,000 |
| Specialty Mushrooms | $0 | $0 | $54,000 | $108,000 | $162,000 |
| Heritage Rabbits | $0 | $0 | $36,000 | $72,000 | $162,000 |
| Total Additional Revenue | =SUM(B10:B12) | =SUM(C10:C12) | =SUM(D10:D12) | =SUM(E10:E12) | =SUM(F10:F12) |

### Total Revenue
| | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|--|--------|--------|--------|--------|--------|
| Total Revenue | =B8+B13 | =C8+C13 | =D8+D13 | =E8+E13 | =F8+F13 |

## Worksheet 3: Monthly Revenue - Year 1

### Monthly Chef Client Growth
| Month | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 |
|-------|---|---|---|---|---|---|---|---|---|----|----|----| 
| Chef Clients | 3 | 4 | 5 | 5 | 6 | 6 | 7 | 7 | 7 | 7 | 7 | 7 |
| Trays per Week | 3 | 3 | 3.5 | 3.5 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 |
| Tray Price | $30 | $30 | $30 | $30 | $30 | $30 | $30 | $30 | $30 | $30 | $30 | $30 |
| Weekly Revenue | =B4*B5*B6 | =C4*C5*C6 | =D4*D5*D6 | =E4*E5*E6 | =F4*F5*F6 | =G4*G5*G6 | =H4*H5*H6 | =I4*I5*I6 | =J4*J5*J6 | =K4*K5*K6 | =L4*L5*L6 | =M4*M5*M6 |
| Monthly Revenue | =B7*4.3 | =C7*4.3 | =D7*4.3 | =E7*4.3 | =F7*4.3 | =G7*4.3 | =H7*4.3 | =I7*4.3 | =J7*4.3 | =K7*4.3 | =L7*4.3 | =M7*4.3 |

### Monthly Trays
| Month | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 |
|-------|---|---|---|---|---|---|---|---|---|----|----|----| 
| Total Trays | =B4*B5*4.3 | =C4*C5*4.3 | =D4*D5*4.3 | =E4*E5*4.3 | =F4*F5*4.3 | =G4*G5*4.3 | =H4*H5*4.3 | =I4*I5*4.3 | =J4*J5*4.3 | =K4*K5*4.3 | =L4*L5*4.3 | =M4*M5*4.3 |

### Cumulative Year 1
| | Total |
|--|-------|
| Total Year 1 Revenue | =SUM(B8:M8) |
| Total Year 1 Trays | =SUM(B11:M11) |

## Worksheet 4: COGS

### Direct Costs per Tray
| Cost Component | Amount |
|----------------|--------|
| Seeds, mats, bamboo | $6.00 |
| Delivery tip (3rd party) | $1.50 |
| Tray return pickup (every 3rd) | $1.50 |
| Sanitizer, water | $0.50 |
| Total COGS per Tray | =SUM(B4:B7) |

### Annual COGS
| Category | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|----------|--------|--------|--------|--------|--------|
| Microgreens COGS | ='Revenue Projections'!B7*'COGS'!B9 | ='Revenue Projections'!C7*'COGS'!B9 | ='Revenue Projections'!D7*'COGS'!B9 | ='Revenue Projections'!E7*'COGS'!B9 | ='Revenue Projections'!F7*'COGS'!B9 |
| Additional Products COGS | ='Revenue Projections'!B13*0.4 | ='Revenue Projections'!C13*0.4 | ='Revenue Projections'!D13*0.4 | ='Revenue Projections'!E13*0.4 | ='Revenue Projections'!F13*0.4 |
| Total COGS | =B11+B12 | =C11+C12 | =D11+D12 | =E11+E12 | =F11+F12 |

## Worksheet 5: OpEx

### Fixed Monthly Expenses
| Expense Category | Amount |
|------------------|--------|
| Rent | $350 |
| Utilities | $150 |
| Insurance + permits | $200 |
| Labor overhead | $600 |
| Total Monthly Fixed Costs | =SUM(B4:B7) |

### Annual Operating Expenses
| Category | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|----------|--------|--------|--------|--------|--------|
| Rent | =B4*12 | =C11*1.03 | =D11*1.03 | =E11*1.03 | =F11*1.03 |
| Utilities | =B5*12 | =C12*1.05 | =D12*1.05 | =E12*1.05 | =F12*1.05 |
| Insurance + Permits | =B6*12 | =C13*1.02 | =D13*1.02 | =E13*1.02 | =F13*1.02 |
| Labor | =B7*12 | =C14*2 | =D14*1.5 | =E14*1.3 | =F14*1.2 |
| Marketing | =5000 | =7500 | =15000 | =25000 | =35000 |
| Equipment Maintenance | =2000 | =3500 | =7000 | =12000 | =18000 |
| Professional Services | =3000 | =4000 | =6000 | =8000 | =10000 |
| Miscellaneous | =2000 | =3000 | =5000 | =7000 | =10000 |
| Total OpEx | =SUM(B11:B18) | =SUM(C11:C18) | =SUM(D11:D18) | =SUM(E11:E18) | =SUM(F11:F18) |

## Worksheet 6: Unit Economics

### Tray Economics
| Metric | Value |
|--------|-------|
| Average Tray Price | $30 |
| COGS per Tray | ='COGS'!B9 |
| Delivery Cost per Tray | $1.50 |
| Gross Profit per Tray | =B4-B5-B6 |
| Gross Margin % | =B7/B4 |

### Chef Economics
| Metric | Value |
|--------|-------|
| Average Weekly Trays per Chef | 4 |
| Weekly Revenue per Chef | =B11*'Unit Economics'!B4 |
| Weekly COGS per Chef | =B11*('Unit Economics'!B5+'Unit Economics'!B6) |
| Weekly Gross Profit per Chef | =B12-B13 |
| Monthly Revenue per Chef | =B12*4.3 |
| Monthly Gross Profit per Chef | =B14*4.3 |
| Annual Revenue per Chef | =B15*12 |
| Annual Gross Profit per Chef | =B16*12 |

## Worksheet 7: Break-even Analysis

### Fixed Costs
| Category | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|----------|--------|--------|--------|--------|--------|
| Monthly Fixed Costs | ='OpEx'!B8 | ='OpEx'!C19/12 | ='OpEx'!D19/12 | ='OpEx'!E19/12 | ='OpEx'!F19/12 |

### Break-even Calculation
| Metric | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|--------|--------|--------|--------|--------|--------|
| Contribution Margin per Tray | ='Unit Economics'!B7 | ='Unit Economics'!B7 | ='Unit Economics'!B7 | ='Unit Economics'!B7 | ='Unit Economics'!B7 |
| Monthly Fixed Costs | =B4 | =C4 | =D4 | =E4 | =F4 |
| Break-even Trays per Month | =B7/B6 | =C7/C6 | =D7/D6 | =E7/E6 | =F7/F6 |
| Break-even Chef Clients | =B9/'Unit Economics'!B11/4.3 | =C9/'Unit Economics'!B11/4.3 | =D9/'Unit Economics'!B11/4.3 | =E9/'Unit Economics'!B11/4.3 | =F9/'Unit Economics'!B11/4.3 |

## Worksheet 8: Cash Flow - Year 1

### Monthly Cash Flow
| Category | Month 1 | Month 2 | Month 3 | Month 4 | Month 5 | Month 6 | Month 7 | Month 8 | Month 9 | Month 10 | Month 11 | Month 12 |
|----------|---------|---------|---------|---------|---------|---------|---------|---------|---------|----------|----------|----------|
| Revenue | ='Monthly Revenue - Year 1'!B8 | ='Monthly Revenue - Year 1'!C8 | ='Monthly Revenue - Year 1'!D8 | ='Monthly Revenue - Year 1'!E8 | ='Monthly Revenue - Year 1'!F8 | ='Monthly Revenue - Year 1'!G8 | ='Monthly Revenue - Year 1'!H8 | ='Monthly Revenue - Year 1'!I8 | ='Monthly Revenue - Year 1'!J8 | ='Monthly Revenue - Year 1'!K8 | ='Monthly Revenue - Year 1'!L8 | ='Monthly Revenue - Year 1'!M8 |
| COGS | ='Monthly Revenue - Year 1'!B11*'COGS'!B9 | ='Monthly Revenue - Year 1'!C11*'COGS'!B9 | ='Monthly Revenue - Year 1'!D11*'COGS'!B9 | ='Monthly Revenue - Year 1'!E11*'COGS'!B9 | ='Monthly Revenue - Year 1'!F11*'COGS'!B9 | ='Monthly Revenue - Year 1'!G11*'COGS'!B9 | ='Monthly Revenue - Year 1'!H11*'COGS'!B9 | ='Monthly Revenue - Year 1'!I11*'COGS'!B9 | ='Monthly Revenue - Year 1'!J11*'COGS'!B9 | ='Monthly Revenue - Year 1'!K11*'COGS'!B9 | ='Monthly Revenue - Year 1'!L11*'COGS'!B9 | ='Monthly Revenue - Year 1'!M11*'COGS'!B9 |
| Gross Profit | =B4-B5 | =C4-C5 | =D4-D5 | =E4-E5 | =F4-F5 | =G4-G5 | =H4-H5 | =I4-I5 | =J4-J5 | =K4-K5 | =L4-L5 | =M4-M5 |
| Fixed Expenses | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 | ='OpEx'!B8 |
| Marketing | =416 | =416 | =416 | =416 | =416 | =416 | =416 | =416 | =416 | =416 | =416 | =416 |
| Equipment Maintenance | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 |
| Professional Services | =250 | =250 | =250 | =250 | =250 | =250 | =250 | =250 | =250 | =250 | =250 | =250 |
| Miscellaneous | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 | =166 |
| Total Expenses | =SUM(B7:B10) | =SUM(C7:C10) | =SUM(D7:D10) | =SUM(E7:E10) | =SUM(F7:F10) | =SUM(G7:G10) | =SUM(H7:H10) | =SUM(I7:I10) | =SUM(J7:J10) | =SUM(K7:K10) | =SUM(L7:L10) | =SUM(M7:M10) |
| Net Cash Flow | =B6-B11 | =C6-C11 | =D6-D11 | =E6-E11 | =F6-F11 | =G6-G11 | =H6-H11 | =I6-I11 | =J6-J11 | =K6-K11 | =L6-L11 | =M6-M11 |
| Cumulative Cash Flow | =B12 | =B13+C12 | =C13+D12 | =D13+E12 | =E13+F12 | =F13+G12 | =G13+H12 | =H13+I12 | =I13+J12 | =J13+K12 | =K13+L12 | =L13+M12 |

## Worksheet 9: Capital Expenditure

### Phase 0.8 Buildout
| Item | Description | Cost |
|------|-------------|------|
| Grow Racks (3 needed) | Modular racks w/ casters | $600 |
| LED Grow Lights | Low-energy, high-output | $300 |
| Magnetic Wall System | Modular grow wall setup | $200 |
| Collapsible Tables/Tools | Harvest station | $250 |
| Cooler (8-ft, seasonal use) | Located on east end of grow zone | $600 |
| Delivery Crates & Tray Tools | Totes, mist bottles, gloves, returns | $100 |
| Water + Power Access | Basic water filter + plug access | $150 |
| Cleaning & Storage | Soap, bins, seed containers | $150 |
| Total Phase 0.8 | | =SUM(B4:B11) |

### Phase 1-3 Capital Expenditures
| Category | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|----------|--------|--------|--------|--------|--------|
| Phase 0.8 Buildout | =B12 | $0 | $0 | $0 | $0 |
| Container Farm Setup | $0 | $49,800 | $0 | $0 | $0 |
| Additional Growing Equipment | $0 | $5,000 | $15,000 | $20,000 | $25,000 |
| Geodesic Dome | $0 | $7,500 | $0 | $0 | $0 |
| Mushroom Growing Facility | $0 | $0 | $5,000 | $0 | $0 |
| Rabbit Husbandry Setup | $0 | $0 | $4,000 | $0 | $0 |
| Renewable Energy Systems | $0 | $0 | $8,000 | $0 | $0 |
| Delivery Vehicle | $0 | $0 | $8,000 | $0 | $12,000 |
| Technology & Software | $0 | $4,000 | $2,000 | $3,000 | $5,000 |
| Total CapEx | =SUM(B15:B23) | =SUM(C15:C23) | =SUM(D15:D23) | =SUM(E15:E23) | =SUM(F15:F23) |

## Worksheet 10: Funding & Investment

### Funding Request
| Category | Amount | Description |
|----------|--------|-------------|
| Phase 0.8 Buildout | $2,350 | Complete initial 5-rack system |
| Container Farm Setup | $49,800 | Phase 1 container retrofit + equipment |
| Working Capital | $10,000 | Inventory, marketing, operations |
| Technology Development | $4,000 | QR tray-tracking app, monitoring systems |
| Contingency | $2,850 | Unexpected expenses and opportunities |
| Total Funding Request | =SUM(B4:B8) | |

### Return on Investment Analysis
| Metric | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|--------|--------|--------|--------|--------|--------|
| Investment | =B9 | $0 | $0 | $0 | $0 |
| Net Income | ='Dashboard'!B12 | ='Dashboard'!C12 | ='Dashboard'!D12 | ='Dashboard'!E12 | ='Dashboard'!F12 |
| Cumulative Net Income | =B12 | =B13+C12 | =C13+D12 | =D13+E12 | =E13+F12 |
| ROI (Cumulative) | =B13/B11 | =C13/B11 | =D13/B11 | =E13/B11 | =F13/B11 |
| Payback Period | =IF(B14>=1,"Year 1",IF(C14>=1,"Year 2",IF(D14>=1,"Year 3",IF(E14>=1,"Year 4",IF(F14>=1,"Year 5","Beyond Year 5"))))) |

## Worksheet 11: Sensitivity Analysis

### Revenue Sensitivity
| Scenario | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|----------|--------|--------|--------|--------|--------|
| Base Case Revenue | ='Dashboard'!B4 | ='Dashboard'!C4 | ='Dashboard'!D4 | ='Dashboard'!E4 | ='Dashboard'!F4 |
| Optimistic (+20%) | =B4*1.2 | =C4*1.2 | =D4*1.2 | =E4*1.2 | =F4*1.2 |
| Pessimistic (-20%) | =B4*0.8 | =C4*0.8 | =D4*0.8 | =E4*0.8 | =F4*0.8 |

### COGS Sensitivity
| Scenario | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|----------|--------|--------|--------|--------|--------|
| Base Case COGS | ='Dashboard'!B5 | ='Dashboard'!C5 | ='Dashboard'!D5 | ='Dashboard'!E5 | ='Dashboard'!F5 |
| Higher COGS (+15%) | =B10*1.15 | =C10*1.15 | =D10*1.15 | =E10*1.15 | =F10*1.15 |
| Lower COGS (-10%) | =B10*0.9 | =C10*0.9 | =D10*0.9 | =E10*0.9 | =F10*0.9 |

### Chef Acquisition Sensitivity
| Scenario | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|----------|--------|--------|--------|--------|--------|
| Base Case Chef Count | ='Revenue Projections'!B4 | ='Revenue Projections'!C4 | ='Revenue Projections'!D4 | ='Revenue Projections'!E4 | ='Revenue Projections'!F4 |
| Faster Acquisition (+25%) | =B16*1.25 | =C16*1.25 | =D16*1.25 | =E16*1.25 | =F16*1.25 |
| Slower Acquisition (-25%) | =B16*0.75 | =C16*0.75 | =D16*0.75 | =E16*0.75 | =F16*0.75 |

### Combined Scenario Analysis
| Scenario | Year 1 | Year 2 | Year 3 | Year 4 | Year 5 |
|----------|--------|--------|--------|--------|--------|
| Base Case Net Income | ='Dashboard'!B12 | ='Dashboard'!C12 | ='Dashboard'!D12 | ='Dashboard'!E12 | ='Dashboard'!F12 |
| Best Case | =(B5*B17-B11*B13)*0.8 | =(C5*C17-C11*C13)*0.8 | =(D5*D17-D11*D13)*0.8 | =(E5*E17-E11*E13)*0.8 | =(F5*F17-F11*F13)*0.8 |
| Worst Case | =(B7*B19-B11*B13)*0.8 | =(C7*C19-C11*C13)*0.8 | =(D7*D19-D11*D13)*0.8 | =(E7*E19-E11*E13)*0.8 | =(F7*F19-F11*F13)*0.8 |

## Worksheet 12: Valuation

### Discounted Cash Flow
| Year | 0 | 1 | 2 | 3 | 4 | 5 |
|------|---|---|---|---|---|---|
| Net Income | | ='Dashboard'!B12 | ='Dashboard'!C12 | ='Dashboard'!D12 | ='Dashboard'!E12 | ='Dashboard'!F12 |
| Capital Expenditures | | ='Capital Expenditure'!B24 | ='Capital Expenditure'!C24 | ='Capital Expenditure'!D24 | ='Capital Expenditure'!E24 | ='Capital Expenditure'!F24 |
| Free Cash Flow | -'Funding & Investment'!B9 | =B5-B6 | =C5-C6 | =D5-D6 | =E5-E6 | =F5-F6 |
| Discount Factor (20%) | 1 | 0.833 | 0.694 | 0.579 | 0.482 | 0.402 |
| Discounted Cash Flow | =B7*B8 | =C7*C8 | =D7*D8 | =E7*E8 | =F7*F8 | =G7*G8 |
| Cumulative DCF | =B9 | =B10+C9 | =C10+D9 | =D10+E9 | =E10+F9 | =F10+G9 |
| NPV | =G10 | | | | | |

### Multiple-Based Valuation (Year 5)
| Metric | Value |
|--------|-------|
| Year 5 Revenue | ='Dashboard'!F4 |
| Revenue Multiple | 2.5 |
| Revenue-Based Valuation | =B14*B15 |
| Year 5 EBITDA | ='Dashboard'!F10 |
| EBITDA Multiple | 8 |
| EBITDA-Based Valuation | =B17*B18 |
| Average Valuation | =(B16+B19)/2 |

### Investor Returns
| Metric | Value |
|--------|-------|
| Initial Investment | ='Funding & Investment'!B9 |
| Ownership Stake | 25% |
| Exit Valuation (Year 5) | =B20 |
| Investor Portion at Exit | =B24*B25 |
| Multiple on Investment | =B26/B23 |
| IRR | =IRR(B9:G7) |