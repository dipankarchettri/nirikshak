# Nirikshak scorecard

False-alarm budget alpha = 5%. Rates show exact 95% intervals in brackets.
Key rate: asymptotic BB84, secret bits per sifted bit; 0 means the protocol would abort.

## Real hardware, per session

### `ibm_kingston` batch 1 (timing not matched, job `dbcdge9gv2cc73ea4ne0`)

Not used for claims: rounds Eve did not touch picked up extra noise.

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 0.7% | 0.7% | 0.88 | 2/20 | 0/20 | 0.5981 | clean |
| honest | 0.8% | 0.7% | 0.87 | 0/20 | 0/20 | 0.3187 | clean |
| honest | 0.7% | 1.0% | 0.87 | 0/20 | 0/20 | 0.9622 | clean |
| intercept 1/16 | 5.7% | 0.9% | 0.37 | 20/20 | 0/20 | 0.0001 | **attack** |
| intercept 2/16 | 5.6% | 0.7% | 0.38 | 20/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 10.8% | 0.8% | 0.01 | 20/20 | 9/20 | 0.0001 | **attack** |
| intercept 8/16 | 16.5% | 0.8% | 0.00 | 20/20 | 19/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 4.3% | 1.0% | 0.49 | 20/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 4.5% | 0.9% | 0.47 | 20/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 5.1% | 0.8% | 0.42 | 20/20 | 0/20 | 0.0001 | **attack** |

### `ibm_kingston` batch 2 (timing matched, plain idle, job `dbcdpek24mrc73cjedeg`)

Not used for claims: plain idle raised the noise floor (superseded by spin echo).

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 4.3% | 4.2% | 0.49 | 0/20 | 0/20 | 0.4022 | clean |
| honest | 3.9% | 4.7% | 0.53 | 0/20 | 0/20 | 0.9709 | clean |
| honest | 4.4% | 4.0% | 0.48 | 3/20 | 0/20 | 0.1602 | clean |
| intercept 1/16 | 6.0% | 4.2% | 0.35 | 6/20 | 0/20 | 0.0008 | **attack** |
| intercept 2/16 | 7.6% | 4.3% | 0.23 | 3/20 | 1/20 | 0.0001 | **attack** |
| intercept 4/16 | 10.8% | 4.2% | 0.01 | 20/20 | 9/20 | 0.0001 | **attack** |
| intercept 8/16 | 15.0% | 4.6% | 0.00 | 20/20 | 20/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 4.1% | 3.2% | 0.51 | 1/20 | 0/20 | 0.0013 | **attack** |
| probe pi/4, 8/16 | 4.2% | 3.0% | 0.50 | 3/20 | 0/20 | 0.0005 | **attack** |
| probe pi/4, 16/16 | 5.5% | 3.0% | 0.39 | 14/20 | 0/20 | 0.0001 | **attack** |

### `ibm_kingston` batch 3 (timing matched, spin echo, job `dbcdsck24mrc73cjek9g`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 1.7% | 1.5% | 0.76 | 0/20 | 0/20 | 0.2361 | clean |
| honest | 1.8% | 1.9% | 0.74 | 0/20 | 0/20 | 0.5776 | clean |
| honest | 1.8% | 2.0% | 0.75 | 0/20 | 0/20 | 0.8721 | clean |
| intercept 1/16 | 3.1% | 1.5% | 0.60 | 12/20 | 0/20 | 0.0001 | **attack** |
| intercept 2/16 | 4.9% | 1.5% | 0.43 | 19/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 7.8% | 1.7% | 0.21 | 20/20 | 1/20 | 0.0001 | **attack** |
| intercept 8/16 | 15.1% | 1.7% | 0.00 | 20/20 | 19/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 4.5% | 1.8% | 0.47 | 20/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 3.8% | 1.9% | 0.53 | 10/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 5.5% | 1.7% | 0.39 | 20/20 | 0/20 | 0.0001 | **attack** |

### `ibm_kingston` batch 4 (timing matched, spin echo, job `dbce8c0c77vs738641j0`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 1.7% | 1.7% | 0.75 | 0/20 | 0/20 | 0.4993 | clean |
| honest | 1.7% | 1.8% | 0.75 | 0/20 | 0/20 | 0.7496 | clean |
| honest | 1.8% | 1.7% | 0.74 | 0/20 | 0/20 | 0.2976 | clean |
| intercept 1/16 | 3.0% | 1.7% | 0.61 | 9/20 | 0/20 | 0.0002 | **attack** |
| intercept 2/16 | 4.8% | 1.8% | 0.45 | 17/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 7.8% | 1.9% | 0.21 | 20/20 | 2/20 | 0.0001 | **attack** |
| intercept 8/16 | 14.2% | 1.7% | 0.00 | 20/20 | 18/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 4.1% | 2.0% | 0.51 | 15/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 3.8% | 1.9% | 0.53 | 15/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 5.2% | 1.8% | 0.41 | 20/20 | 0/20 | 0.0001 | **attack** |

### `ibm_kingston` batch 5 (timing matched, spin echo, job `dbd0vo424mrc73cki1l0`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 1.7% | 1.7% | 0.75 | 3/20 | 0/20 | 0.5273 | clean |
| honest | 1.7% | 1.5% | 0.75 | 2/20 | 0/20 | 0.1687 | clean |
| honest | 1.9% | 1.8% | 0.73 | 3/20 | 0/20 | 0.3774 | clean |
| intercept 1/16 | 3.2% | 1.8% | 0.59 | 7/20 | 0/20 | 0.0001 | **attack** |
| intercept 2/16 | 5.1% | 1.8% | 0.42 | 18/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 8.5% | 1.8% | 0.16 | 20/20 | 4/20 | 0.0001 | **attack** |
| intercept 8/16 | 15.4% | 1.9% | 0.00 | 20/20 | 20/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 3.7% | 1.9% | 0.54 | 15/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 3.7% | 2.0% | 0.55 | 12/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 5.3% | 2.0% | 0.41 | 19/20 | 0/20 | 0.0001 | **attack** |

### `ibm_fez` batch 6 (timing matched, spin echo, job `dbd104pgv2cc738h5m80`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 1.9% | 1.8% | 0.72 | 1/20 | 0/20 | 0.2814 | clean |
| honest | 1.9% | 2.0% | 0.73 | 0/20 | 0/20 | 0.7557 | clean |
| honest | 2.2% | 1.9% | 0.70 | 4/20 | 0/20 | 0.0972 | clean |
| intercept 1/16 | 3.2% | 2.2% | 0.59 | 7/20 | 0/20 | 0.0004 | **attack** |
| intercept 2/16 | 5.2% | 2.0% | 0.41 | 19/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 7.6% | 1.9% | 0.22 | 20/20 | 1/20 | 0.0001 | **attack** |
| intercept 8/16 | 13.5% | 2.0% | 0.00 | 20/20 | 17/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 4.6% | 2.7% | 0.46 | 13/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 4.3% | 2.9% | 0.49 | 7/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 5.7% | 2.8% | 0.37 | 18/20 | 0/20 | 0.0001 | **attack** |

### `ibm_marrakesh` batch 7 (timing matched, spin echo, job `dbd3bts24mrc73cklb10`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 3.5% | 3.4% | 0.56 | 0/20 | 0/20 | 0.3206 | clean |
| honest | 3.9% | 3.8% | 0.52 | 2/20 | 0/20 | 0.2837 | clean |
| honest | 3.5% | 3.8% | 0.56 | 0/20 | 0/20 | 0.8839 | clean |
| intercept 1/16 | 4.9% | 3.9% | 0.43 | 1/20 | 0/20 | 0.0035 | **attack** |
| intercept 2/16 | 7.0% | 3.2% | 0.27 | 17/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 9.5% | 3.6% | 0.10 | 20/20 | 2/20 | 0.0001 | **attack** |
| intercept 8/16 | 15.0% | 3.1% | 0.00 | 20/20 | 19/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 10.2% | 3.6% | 0.05 | 20/20 | 8/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 7.6% | 3.6% | 0.22 | 19/20 | 2/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 11.4% | 3.7% | 0.00 | 20/20 | 11/20 | 0.0001 | **attack** |

### `ibm_kingston` batch 8 (timing matched, spin echo, job `dbkpimlgg49c73djdno0`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 1.6% | 1.6% | 0.76 | 0/20 | 0/20 | 0.4181 | clean |
| honest | 1.9% | 1.7% | 0.73 | 1/20 | 0/20 | 0.1575 | clean |
| honest | 1.7% | 1.6% | 0.75 | 1/20 | 0/20 | 0.3429 | clean |
| honest | 1.7% | 1.7% | 0.75 | 1/20 | 0/20 | 0.3299 | clean |
| honest | 1.6% | 1.7% | 0.77 | 0/20 | 0/20 | 0.7408 | clean |
| honest | 1.7% | 1.7% | 0.75 | 1/20 | 0/20 | 0.3654 | clean |
| honest | 1.7% | 1.5% | 0.75 | 0/20 | 0/20 | 0.1732 | clean |
| honest | 1.7% | 1.5% | 0.75 | 2/20 | 0/20 | 0.1798 | clean |
| honest | 1.5% | 1.4% | 0.78 | 1/20 | 0/20 | 0.3564 | clean |
| honest | 1.7% | 1.8% | 0.76 | 0/20 | 0/20 | 0.7970 | clean |
| intercept 1/16 | 2.9% | 1.4% | 0.62 | 14/20 | 0/20 | 0.0001 | **attack** |
| intercept 2/16 | 4.5% | 1.6% | 0.47 | 19/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 8.3% | 1.7% | 0.18 | 20/20 | 4/20 | 0.0001 | **attack** |
| intercept 8/16 | 14.8% | 1.4% | 0.00 | 20/20 | 18/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 8.2% | 2.2% | 0.18 | 20/20 | 1/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 7.4% | 2.1% | 0.24 | 20/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 9.0% | 1.9% | 0.13 | 20/20 | 1/20 | 0.0001 | **attack** |

### `ibm_fez` batch 9 (timing matched, spin echo, job `dbkpipgnceqs73amdc10`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 2.3% | 2.3% | 0.68 | 2/20 | 0/20 | 0.4847 | clean |
| honest | 2.6% | 2.2% | 0.65 | 5/20 | 0/20 | 0.0201 | **attack** |
| honest | 2.5% | 2.8% | 0.66 | 1/20 | 0/20 | 0.8359 | clean |
| honest | 3.1% | 2.6% | 0.60 | 5/20 | 0/20 | 0.0484 | **attack** |
| honest | 2.7% | 2.4% | 0.64 | 0/20 | 0/20 | 0.1773 | clean |
| honest | 2.6% | 2.4% | 0.65 | 0/20 | 0/20 | 0.2417 | clean |
| honest | 2.4% | 2.6% | 0.67 | 1/20 | 0/20 | 0.7080 | clean |
| honest | 2.3% | 2.4% | 0.69 | 0/20 | 0/20 | 0.8030 | clean |
| honest | 2.5% | 2.2% | 0.67 | 4/20 | 0/20 | 0.1844 | clean |
| honest | 2.3% | 2.5% | 0.69 | 0/20 | 0/20 | 0.8781 | clean |
| intercept 1/16 | 3.8% | 2.6% | 0.54 | 9/20 | 0/20 | 0.0008 | **attack** |
| intercept 2/16 | 5.8% | 2.5% | 0.36 | 19/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 8.5% | 2.5% | 0.16 | 20/20 | 1/20 | 0.0001 | **attack** |
| intercept 8/16 | 14.0% | 2.4% | 0.00 | 20/20 | 17/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 4.8% | 3.0% | 0.45 | 8/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 4.9% | 2.8% | 0.44 | 9/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 5.9% | 3.1% | 0.36 | 12/20 | 0/20 | 0.0001 | **attack** |

### `ibm_marrakesh` batch 10 (timing matched, spin echo, job `dbkpit9kdqps7392v7mg`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 4.4% | 5.1% | 0.48 | 0/20 | 0/20 | 0.9595 | clean |
| honest | 4.6% | 4.6% | 0.46 | 0/20 | 0/20 | 0.5180 | clean |
| honest | 4.9% | 4.7% | 0.44 | 1/20 | 0/20 | 0.2899 | clean |
| honest | 4.8% | 4.6% | 0.44 | 1/20 | 0/20 | 0.2286 | clean |
| honest | 4.8% | 4.4% | 0.45 | 0/20 | 0/20 | 0.1095 | clean |
| honest | 4.7% | 4.4% | 0.46 | 3/20 | 0/20 | 0.1838 | clean |
| honest | 4.8% | 4.7% | 0.44 | 0/20 | 0/20 | 0.4286 | clean |
| honest | 4.9% | 4.6% | 0.43 | 1/20 | 0/20 | 0.2034 | clean |
| honest | 4.5% | 4.5% | 0.47 | 1/20 | 0/20 | 0.4209 | clean |
| honest | 4.8% | 4.4% | 0.44 | 1/20 | 0/20 | 0.0649 | clean |
| intercept 1/16 | 6.1% | 4.1% | 0.34 | 12/20 | 0/20 | 0.0001 | **attack** |
| intercept 2/16 | 7.8% | 4.5% | 0.21 | 17/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 10.0% | 4.1% | 0.06 | 19/20 | 8/20 | 0.0001 | **attack** |
| intercept 8/16 | 15.5% | 4.3% | 0.00 | 20/20 | 19/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 6.7% | 4.2% | 0.29 | 16/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 6.6% | 4.1% | 0.30 | 14/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 8.4% | 4.0% | 0.17 | 19/20 | 0/20 | 0.0001 | **attack** |

### `ibm_kingston` batch 11 (timing matched, spin echo, job `dbkpnblgg49c73dje1h0`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 1.6% | 1.6% | 0.76 | 5/20 | 0/20 | 0.4277 | clean |
| honest | 1.5% | 1.5% | 0.78 | 0/20 | 0/20 | 0.6229 | clean |
| honest | 1.6% | 1.8% | 0.76 | 0/20 | 0/20 | 0.8443 | clean |
| honest | 1.5% | 1.6% | 0.78 | 0/20 | 0/20 | 0.7654 | clean |
| honest | 1.4% | 1.3% | 0.79 | 2/20 | 0/20 | 0.2957 | clean |
| honest | 1.7% | 1.6% | 0.75 | 0/20 | 0/20 | 0.2483 | clean |
| honest | 1.5% | 1.4% | 0.78 | 1/20 | 0/20 | 0.4470 | clean |
| honest | 1.6% | 1.6% | 0.77 | 0/20 | 0/20 | 0.5496 | clean |
| honest | 1.6% | 1.6% | 0.76 | 3/20 | 0/20 | 0.3249 | clean |
| honest | 1.7% | 1.4% | 0.76 | 1/20 | 0/20 | 0.1444 | clean |
| intercept 1/16 | 3.1% | 1.5% | 0.60 | 13/20 | 0/20 | 0.0001 | **attack** |
| intercept 2/16 | 4.7% | 1.7% | 0.45 | 18/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 7.9% | 1.3% | 0.20 | 20/20 | 2/20 | 0.0001 | **attack** |
| intercept 8/16 | 14.5% | 1.4% | 0.00 | 20/20 | 16/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 8.3% | 2.0% | 0.17 | 20/20 | 3/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 6.7% | 2.3% | 0.29 | 20/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 9.5% | 2.2% | 0.09 | 20/20 | 3/20 | 0.0001 | **attack** |

### `ibm_fez` batch 12 (timing matched, spin echo, job `dbkpngt6p51s73cn5fpg`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 2.4% | 2.3% | 0.67 | 0/20 | 0/20 | 0.3514 | clean |
| honest | 2.1% | 2.2% | 0.70 | 0/20 | 0/20 | 0.5586 | clean |
| honest | 2.6% | 2.6% | 0.65 | 1/20 | 0/20 | 0.4888 | clean |
| honest | 2.7% | 2.4% | 0.64 | 1/20 | 0/20 | 0.1084 | clean |
| honest | 2.6% | 2.6% | 0.65 | 0/20 | 0/20 | 0.5360 | clean |
| honest | 2.4% | 2.5% | 0.67 | 1/20 | 0/20 | 0.6413 | clean |
| honest | 2.5% | 2.2% | 0.66 | 1/20 | 0/20 | 0.0973 | clean |
| honest | 2.5% | 2.4% | 0.66 | 0/20 | 0/20 | 0.3018 | clean |
| honest | 2.4% | 2.4% | 0.67 | 3/20 | 0/20 | 0.5101 | clean |
| honest | 2.7% | 2.3% | 0.64 | 1/20 | 0/20 | 0.0161 | **attack** |
| intercept 1/16 | 3.6% | 2.5% | 0.56 | 4/20 | 0/20 | 0.0003 | **attack** |
| intercept 2/16 | 5.4% | 2.4% | 0.39 | 19/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 9.3% | 2.4% | 0.11 | 20/20 | 4/20 | 0.0001 | **attack** |
| intercept 8/16 | 14.9% | 2.7% | 0.00 | 20/20 | 18/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 5.1% | 3.3% | 0.42 | 11/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 4.6% | 2.7% | 0.46 | 8/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 6.0% | 2.8% | 0.34 | 15/20 | 0/20 | 0.0001 | **attack** |

### `ibm_marrakesh` batch 13 (timing matched, spin echo, job `dbkpnkdgg49c73dje2b0`)

| Session | Key QBER | Reference QBER | Key rate | Nirikshak blocks | 11% rule blocks | Session p-value | Session verdict |
| :--- | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| honest | 4.6% | 4.8% | 0.47 | 0/20 | 0/20 | 0.7856 | clean |
| honest | 4.4% | 4.9% | 0.48 | 0/20 | 0/20 | 0.9305 | clean |
| honest | 5.3% | 4.7% | 0.40 | 3/20 | 0/20 | 0.0425 | **attack** |
| honest | 4.4% | 4.9% | 0.48 | 0/20 | 0/20 | 0.9559 | clean |
| honest | 4.9% | 4.7% | 0.44 | 3/20 | 0/20 | 0.2128 | clean |
| honest | 4.8% | 4.4% | 0.44 | 0/20 | 0/20 | 0.1406 | clean |
| honest | 4.6% | 4.5% | 0.46 | 0/20 | 0/20 | 0.4114 | clean |
| honest | 4.6% | 4.5% | 0.47 | 0/20 | 0/20 | 0.4844 | clean |
| honest | 5.1% | 4.6% | 0.41 | 4/20 | 0/20 | 0.1012 | clean |
| honest | 4.2% | 4.7% | 0.50 | 0/20 | 0/20 | 0.9174 | clean |
| intercept 1/16 | 5.9% | 4.9% | 0.36 | 3/20 | 0/20 | 0.0080 | **attack** |
| intercept 2/16 | 7.1% | 4.9% | 0.26 | 4/20 | 0/20 | 0.0001 | **attack** |
| intercept 4/16 | 11.0% | 4.9% | 0.00 | 20/20 | 10/20 | 0.0001 | **attack** |
| intercept 8/16 | 15.7% | 4.8% | 0.00 | 20/20 | 20/20 | 0.0001 | **attack** |
| probe pi/8, 16/16 | 6.7% | 3.9% | 0.29 | 19/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 8/16 | 5.3% | 3.8% | 0.40 | 7/20 | 0/20 | 0.0001 | **attack** |
| probe pi/4, 16/16 | 8.5% | 3.7% | 0.16 | 20/20 | 1/20 | 0.0001 | **attack** |

## Real hardware, `ibm_fez`, pooled over 3 spin-echo batch(es)

Honest row: false alarms. Other rows: detection.

| Condition | Blocks | Nirikshak, per block | 11% rule, per block | Nirikshak, per session |
| :--- | :-: | :-: | :-: | :-: |
| honest | 460 | 7% (5%-9%) | 0% (0%-1%) | 13% (3%-34%) |
| intercept 1/16 | 60 | 33% (22%-47%) | 0% (0%-6%) | 100% (29%-100%) |
| intercept 2/16 | 60 | 95% (86%-99%) | 0% (0%-6%) | 100% (29%-100%) |
| intercept 4/16 | 60 | 100% (94%-100%) | 10% (4%-21%) | 100% (29%-100%) |
| intercept 8/16 | 60 | 100% (94%-100%) | 87% (75%-94%) | 100% (29%-100%) |
| probe pi/8, 16/16 | 60 | 53% (40%-66%) | 0% (0%-6%) | 100% (29%-100%) |
| probe pi/4, 8/16 | 60 | 40% (28%-53%) | 0% (0%-6%) | 100% (29%-100%) |
| probe pi/4, 16/16 | 60 | 75% (62%-85%) | 0% (0%-6%) | 100% (29%-100%) |

## Real hardware, `ibm_kingston`, pooled over 5 spin-echo batch(es)

Honest row: false alarms. Other rows: detection.

| Condition | Blocks | Nirikshak, per block | 11% rule, per block | Nirikshak, per session |
| :--- | :-: | :-: | :-: | :-: |
| honest | 580 | 5% (3%-7%) | 0% (0%-1%) | 0% (0%-12%) |
| intercept 1/16 | 100 | 55% (45%-65%) | 0% (0%-4%) | 100% (48%-100%) |
| intercept 2/16 | 100 | 91% (84%-96%) | 0% (0%-4%) | 100% (48%-100%) |
| intercept 4/16 | 100 | 100% (96%-100%) | 13% (7%-21%) | 100% (48%-100%) |
| intercept 8/16 | 100 | 100% (96%-100%) | 91% (84%-96%) | 100% (48%-100%) |
| probe pi/8, 16/16 | 100 | 90% (82%-95%) | 4% (1%-10%) | 100% (48%-100%) |
| probe pi/4, 8/16 | 100 | 77% (68%-85%) | 0% (0%-4%) | 100% (48%-100%) |
| probe pi/4, 16/16 | 100 | 99% (95%-100%) | 4% (1%-10%) | 100% (48%-100%) |

## Real hardware, `ibm_marrakesh`, pooled over 3 spin-echo batch(es)

Honest row: false alarms. Other rows: detection.

| Condition | Blocks | Nirikshak, per block | 11% rule, per block | Nirikshak, per session |
| :--- | :-: | :-: | :-: | :-: |
| honest | 460 | 4% (3%-7%) | 0% (0%-1%) | 4% (0%-22%) |
| intercept 1/16 | 60 | 27% (16%-40%) | 0% (0%-6%) | 100% (29%-100%) |
| intercept 2/16 | 60 | 63% (50%-75%) | 0% (0%-6%) | 100% (29%-100%) |
| intercept 4/16 | 60 | 98% (91%-100%) | 33% (22%-47%) | 100% (29%-100%) |
| intercept 8/16 | 60 | 100% (94%-100%) | 97% (88%-100%) | 100% (29%-100%) |
| probe pi/8, 16/16 | 60 | 92% (82%-97%) | 13% (6%-25%) | 100% (29%-100%) |
| probe pi/4, 8/16 | 60 | 67% (53%-78%) | 3% (0%-12%) | 100% (29%-100%) |
| probe pi/4, 16/16 | 60 | 98% (91%-100%) | 20% (11%-32%) | 100% (29%-100%) |

## Simulation, session verdict

Honest rows: share of honest sessions wrongly flagged (target 5% or less).

### training conditions

| Condition | Sessions | Session verdict | Per block (Nirikshak) |
| :--- | :-: | :-: | :-: |
| honest | 30 | 13% (4%-31%) | 7% (5%-9%) |
| intercept 1/16 | 10 | 100% (69%-100%) | 51% (44%-58%) |
| intercept 2/16 | 10 | 100% (69%-100%) | 90% (84%-93%) |
| intercept 4/16 | 10 | 100% (69%-100%) | 100% (98%-100%) |
| intercept 8/16 | 10 | 100% (69%-100%) | 100% (98%-100%) |
| probe pi/8, 16/16 | 10 | 100% (69%-100%) | 21% (16%-27%) |
| probe pi/4, 8/16 | 10 | 100% (69%-100%) | 48% (41%-55%) |
| probe pi/4, 16/16 | 10 | 100% (69%-100%) | 80% (73%-85%) |

### drifted noise

| Condition | Sessions | Session verdict | Per block (Nirikshak) |
| :--- | :-: | :-: | :-: |
| honest | 15 | 0% (0%-22%) | 2% (1%-5%) |
| intercept 1/16 | 5 | 80% (28%-99%) | 31% (22%-41%) |
| intercept 2/16 | 5 | 100% (48%-100%) | 60% (50%-70%) |
| intercept 4/16 | 5 | 100% (48%-100%) | 92% (85%-96%) |
| intercept 8/16 | 5 | 100% (48%-100%) | 100% (96%-100%) |
| probe pi/8, 16/16 | 5 | 80% (28%-99%) | 30% (21%-40%) |
| probe pi/4, 8/16 | 5 | 60% (15%-95%) | 18% (11%-27%) |
| probe pi/4, 16/16 | 5 | 100% (48%-100%) | 47% (37%-57%) |

### Kingston noise snapshot

| Condition | Sessions | Session verdict | Per block (Nirikshak) |
| :--- | :-: | :-: | :-: |
| honest | 6 | 0% (0%-46%) | 8% (3%-14%) |
| intercept 1/16 | 2 | 100% (16%-100%) | 78% (62%-89%) |
| intercept 2/16 | 2 | 100% (16%-100%) | 100% (91%-100%) |
| intercept 4/16 | 2 | 100% (16%-100%) | 100% (91%-100%) |
| intercept 8/16 | 2 | 100% (16%-100%) | 100% (91%-100%) |
| probe pi/8, 16/16 | 2 | 100% (16%-100%) | 100% (91%-100%) |
| probe pi/4, 8/16 | 2 | 100% (16%-100%) | 98% (87%-100%) |
| probe pi/4, 16/16 | 2 | 100% (16%-100%) | 100% (91%-100%) |

### drifted noise, honest sessions only

| Condition | Sessions | Session verdict | Per block (Nirikshak) |
| :--- | :-: | :-: | :-: |
| honest | 200 | 6% (4%-11%) | 4% (4%-5%) |

### training conditions, honest sessions only

| Condition | Sessions | Session verdict | Per block (Nirikshak) |
| :--- | :-: | :-: | :-: |
| honest | 400 | 5% (3%-8%) | 5% (4%-5%) |
