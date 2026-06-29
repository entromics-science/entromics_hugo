+++
title = 'Time to Disease Onset and Survival Prognosis in Cancer'
date = 2026-03-04T07:07:07+01:00
draft = false
+++

{{< figure
  src="banner.jpg"
  alt="Time to disease onset and Fisher information analysis"
>}}

<hr>

This application uses results published in the book **B. Roy Frieden, *Science
from Fisher Information. A Unification*, Cambridge University Press, 2004,
chapters 1, 14, 15**. The complete mathematical derivation of the determination
of individual times to the onset of hepatocellular cancer growth, using the
tumor masses (as determined for respective patients by CT imaging at the
"baseline" clinical examination), can be found in the
[text, linked HERE](Fisher-information.pdf).

{{< figure src="HCCS1.JPG" alt="Time to onset and survival prognosis — slide 1" >}}

{{< figure src="HCCS2.JPG" alt="Time to onset and survival prognosis — slide 2" >}}

{{< figure src="HCCS3.JPG" alt="Time to onset and survival prognosis — slide 3" >}}

{{< figure src="HCCS4.JPG" alt="Time to onset and survival prognosis — slide 4" >}}

{{< figure src="HCCFi1.JPG" alt="Fisher information analysis of tumor mass — figure 1" >}}

{{< figure src="HCCFi2.JPG" alt="Fisher information analysis of tumor mass — figure 2" >}}

For details of the following result, see
[the derivation, eq. (24–26), page 6](Fisher-information.pdf).

{{< figure src="HCCFi3_0.JPG" alt="Fisher information analysis of tumor mass — figure 3" >}}

For details of the following result, see
[the derivation, eq. (32–33), page 8](Fisher-information.pdf).

{{< figure src="HCCFi4_0.JPG" alt="Fisher information analysis of tumor mass — figure 4" >}}

The "threshold" tumor mass of 70 resulted from the fact that the linear fit of
the actual log-log transformed data, using two linear relationships, is
statistically significantly better than fitting the same data by just one linear
function. These two relationships (black and blue points, right panel below)
have a threshold at ln(4.25), corresponding to Tmass = 70. The ratio of ~3 for
the tumorigenesis processes in tumors with mass up to 70, compared to larger
tumors, follows from the derived expression for the power constant — see
[eq. (41) in the derivation, page 10](Fisher-information.pdf) — into which we
entered the numerical values obtained from linear fits of the two sets of data
points in the log-log transformed Tmass histogram.

{{< figure src="HCCFi5.JPG" alt="Threshold tumor mass and tumorigenesis rate ratio" >}}

The following result is obtained by
[the derivation, eq. (49–51), page 12](Fisher-information.pdf).

{{< figure src="HCCFi6_2.JPG" alt="Fisher information analysis of tumor mass — figure 6" >}}

For details, see [the derivation, pages 14–15](Fisher-information.pdf).

{{< figure src="HCCFi7_1.JPG" alt="Fisher information analysis of tumor mass — figure 7" >}}

{{< figure src="HCCFi8.JPG" alt="Fisher information analysis of tumor mass — figure 8" >}}

{{< figure src="HCCFi9.JPG" alt="Fisher information analysis of tumor mass — figure 9" >}}

An important practical result, which brings us closer to calculating survival
from baseline diagnosis of individual patients, is that there is a simple linear
relationship between the difference of the personal coherence profile (found for
any patient at baseline) from the "all low" common-data-value reference profile
(HL<sub>1</sub>) and the mean time <em>&lt;t<sub>onset</sub>&gt;</em> that has
passed from disease onset until clinical diagnosis. As we found that all HCC
patients have the same mean total disease duration (<em>OVS<sub>C</sub></em> ~
1045 days), survival prognosis for every one of the 15 possible clinical
statuses of any patient can be determined simply, as shown below.

{{< figure src="HCCFi10_4.jpg" alt="Linear relationship between personal coherence profile and time since disease onset" >}}

A worksheet implementation of this personalized HCC survival prognosis, as
[described in the paper](Pancoska_Tmass_Time_To_Onset_HCC.pdf), is available for
[download](HCC_Survival_Tbaseline.xlsx). Below is a screenshot summarizing the
functions of this tool.

{{< figure src="HCCFi12.jpg" alt="Screenshot of the HCC survival-prognosis worksheet tool" >}}

Because Fisher information processing of the baseline clinical data is not
empirical, it provides important mechanistic insights into the tumor-growth
process, which can be used for hypothesis generation and/or validation:

{{< figure src="HCCFi11.jpg" alt="Mechanistic insights into tumor growth from Fisher information processing" >}}
