# Banking-Regulations-Analysis

In this repository is presented the analysis and assessment of the capital requirement of our credit portfolio, all the definitions and calculations are based on [Basel Committee on Banking Supervision](https://www.bis.org/bcbs/irbriskweight.pdf) and Office of The Superintendent of Financial Institutions documentations ([OSFI](https://www.osfi-bsif.gc.ca/Eng/fi-if/rg-ro/gdn-ort/gl-ld/Pages/CAR19_chpt6.aspx)). The capital requirement calculated was for a bank which portfolio is composed by retail, mortgages and corporate exposures, the foundational and standard approach were used and the Basel III PDs and LGDs were applied.

## Capital Adequacy under the Internal Ratings Based Approach (IRB).

### Exposure at Default

The total exposure at default of the portfolio was $56,759 million CAD. 

For the loans portfolio, considering monthly payments it was required to find the amount of payment by using the formula of an immediate annuity, the remaining payments were bring to present value converting the yearly rate to a monthly effective interest rate, hence the result the loan outstanding balance. By adding each one of these results the EAD of our loan portfolio resulted in $102.17 million dollars.

For the mortgages portfolio, considering monthly payments and converting the annual rate to a monthly effective interest rate, first the value of the payment was calculated using the formula of an immediate annuity, then the standing amount was calculated taking into consideration only the remaining installments minus the collateral, if the exposure was negative the minimum value considered was zero. Thus, the EAD of our mortgage portfolio resulted in $4,507.96 million dollars.

Now for the corporate bonds portfolio, it was used the equivalent rate of a bond which pay yearly coupons, the exposure was calculated by bringing to present value the remaining coupons using the market rate yields ([Canada's bond rate](https://www.bankofcanada.ca/rates/interest-rates/canadian-bonds/)) multiplied by the total of bonds held and divided by 100 because the prices were in cents. Hence, the total EAD of our bond portfolio resulted in $52,599.23 million dollars.

### Expected Loss

The total provisions of the portfolio are $6,445.11 million CAD. The expected loss is the result of the EAD multiplied by the probability of default, for the retail and corporate exposure, it was considered a minimum probability of default of 0.03% (OSFI, 2017).

### Unexpected Loss

The total unexpected loss of the portfolio is $8,918.42 million dollars. 

The unexpected loss is the result of the EAD multiplied by the capital needed. The capital was calculated using the internal rating-based formula (BCBS, 2017); for the loans it was considered an loss given default (LGD) of 100% and a correlation for other retail exposures that allows  the correlation to fluctuate with the probability of default (BCBS, 2017); the mortgages considered a minimum LGD of 10% and the correlation parameter used is of 0.15 (BCBS, 2017).

The UL of the bond portfolio considered the maturity adjustment, a minimum LGD of 45% from IRB Risk Weights for UL (OSFI, 2017) and an adjustment correlation asset was applied (BCBS, 2017). 

### Risk Weighted Assets and Capital Adequacy

The RWAs for the defaulted exposure of the portfolio is of $111,480.28 million CAD. These amounts are the result of the product of the capital, the EAD and a coefficient of 12.5 (BCBS, 2017).

For this exercise the capital requirement that the bank must satisfied according to OSFI is 11.5% of its risk weighted assets resulting in a total of $12,820.23 million CAD.

### Capital Adequacy under the Standard Approach

The RWAs using the standard approach is $42,772.28 million CAD. The method uses the multiplication of the EAD by the weights as specified in OSFI. For the loans the risk weight used was 75%, for the mortgages the risk weight was 35% and for the bonds the risk weight depended on their PD and rating giving in the coursework. Because the bank must satisfy 11.5% of its RWAs the capital requirement is $4,918.81 million CAD.

In comparison with the total risk weighted assets of the third quarter Pillar 3 report of JPMorgan Chase & Co (September 2018), being around $1,438 million dollars the RWA of this bank only represents 2.92% of theirs; evidently, this bank is 33 times smaller compared with magnitude of JP Morgan portfolio. 

The code that contains all the analysis can be found [here](https://github.com/dborgesm/Banking-Regulations/blob/master/Banking_Regulations.ipynb).






