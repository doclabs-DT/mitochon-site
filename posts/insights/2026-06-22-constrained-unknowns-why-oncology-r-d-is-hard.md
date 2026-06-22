---
title: "Constrained Unknowns: Why Oncology R&D is Hard"
date: 2026-06-22T11:59:00.000+01:00
tag: bd
excerpt: You can look up an unknown. You can't look up an optimum
featured: false
---
Almost every conversation about pharmaceutical R&D productivity is, at bottom, a conversation about friction. Trials take too long to enroll. Decisions wait on committees. Data moves slowly between functions. Capital is allocated cautiously. These are real problems and they are worth attacking - but they are also, in an important sense, the *easy* part of the story, because they are in principle fixable - not easy, but fixable. You can compress a timeline. You can shorten a decision. You can rewire an organization.

This essay is about the part you can't fix that way. Let's set aside, for the length of this piece, every human and organizational factor. Imagine a program with perfect execution, instant decisions, and unlimited patience. Oncology drug development would *still* be one of the hardest optimization problems any industry attempts - and the reason has nothing to do with how fast anyone works. It has to do with the structure of what is being optimized.

#### Two kinds of unknown

It helps to separate two species of "unknown," because they behave completely differently.

The first is an **open unknown**. You don't know a data point, but the moment you measure it, uncertainty collapses, and the right action is obvious because value runs in one direction. Is the compound potent? Does it engage its target? Is it orally bioavailable? You want more potency, more engagement, more bioavailability. More information always helps, and the optimum is at a boundary. Open unknowns are, in the deepest sense, *lookup* problems: hard to answer, but conceptually simple once answered.

The second is a **constrained unknown** - and this is where oncology spends most of its life. Here the optimum is not at a *boundary* but in the *interior*. Too little is bad; too much is also bad; value peaks somewhere in the middle. You cannot optimize a constrained unknown by pushing, because pushing in either direction eventually makes things worse. You have to *locate a peak*. And you can look up an unknown, but you cannot look up an optimum.

#### The master example, and then some observations

The cleanest constrained unknown in all of drug development is **dose**. Too little drug and there is no efficacy. Too much and the toxicity is unacceptable. The best dose lies between, where benefit is adequate and harm is tolerable - and, critically, that point is almost never the maximum tolerated dose. The entire history of cytotoxic chemotherapy assumed otherwise (more is better, dose to the limit of tolerability), and the entire modern correction - the FDA's Project Optimus - exists because for targeted and immuno-oncology agents the efficacy curve often plateaus well below the toxic ceiling. The optimum is interior, and we spent decades dosing past it.

![Figure 1 - The dose trade-off. Efficacy rises and plateaus; toxicity rises and keeps climbing. The optimal dose sits inside the therapeutic window, below the maximum tolerated dose.](/images/uploads/fig1_dose_tradeoff-3.svg)

*Figure 1 (schematic). The optimum is interior: peak benefit–risk sits where efficacy has plateaued but toxicity is still low - to the left of the maximum tolerated dose.*

Once you see the shape, you see it everywhere:

* **The patient population.** A predictive biomarker has a cut-point. Tighten it and you concentrate responders, raising the observed effect - but you shrink the eligible population toward commercial and operational nonviability, and you begin excluding patients who would have benefited. Loosen it and you gain reach but dilute the average effect and raise the risk of a failed or unconvincing trial. The optimal cutoff is interior.
* **The label.** Breadth trades reach against the dilution of the average effect and against regulatory risk. Too narrow leaves patients and value unaddressed; too broad invites a thinner, more contestable benefit. Interior again.
* **The combination.** Adding a partner agent can lift efficacy, but it stacks toxicity and narrows the combined therapeutic window. The right intensity is a peak, not a maximum.
* **The molecule itself.** Binding affinity has an optimum (too weak underengages; too tight drives on-target toxicity in healthy tissue and removes your ability to titrate - and some modalities show an outright bell-shaped response). Half-life has an optimum (too short loses coverage; too long accumulates and cannot be withdrawn when an adverse event appears). Selectivity has an optimum (too promiscuous adds off-target harm; too clean may miss the redundancy that drives the disease). These are designed-in, intrinsic peaks.
* **Even the trial and the price.** How large a study balances statistical confidence against time, cost, and patients exposed. What price balances value capture against access and volume. Interior optima, both.

The enterprise, in other words, is not one Goldilocks problem. It is a *stack* of them.

![Figure 2 - The biomarker-cutoff trade-off. Tightening the cutoff lifts the effect size but shrinks the eligible population; the resulting overall value peaks in the interior.](/images/uploads/fig2_biomarker_cutoff-3.svg)

*Figure 2 (schematic). The same interior optimum, a completely different lever: as the biomarker cutoff tightens, effect size rises while the eligible population falls, and the value that depends on both turns over in the middle.*

#### Why interior optima are intrinsically hard

If these were ordinary unknowns, the stack would still be a lot of work, but it would be tractable: measure each one, push to the edge, move on. They are not ordinary unknowns, and three structural features make them genuinely hard — hard in a way no organizational improvement touches.

**First, you have to visit the bad side to find the peak.** To locate an interior optimum you must characterize *both* of its slopes, which means generating data in the region where things get worse — dosing into toxicity to find the ceiling, and dosing across the efficacy plateau to learn where benefit stops rising. The most informative experiments are precisely the ones you are most reluctant, ethically and practically, to run. With an open unknown you can sample wherever is convenient; with a constrained optimum the decisive samples sit on the far side of harm. This is exactly why dose escalation characterizes the toxic limb beautifully and the efficacy limb barely at all — the design is built to find the edge it is safe to find.

**Second, the slope that matters resolves last.** The cost arm - toxicity - appears early, unambiguously, and at small sample size; Phase 1 is engineered to surface it. The benefit arm - response, durability, survival, real-world value - appears late, noisily, through surrogate endpoints, and only at scale. So at the very moment a program must commit to a dose, a population, an indication, it can see one wall of the canyon in sharp relief and is guessing at the other. The decision that most determines an asset's fate is made with the least-resolved half of the information, and no amount of speed brings the slow half forward - the biology takes the time it takes.

**Third, the peak moves.** A Goldilocks point is not a fixed property of the molecule waiting to be discovered. It is conditioned on everything around it. The optimal dose in monotherapy is not the optimal dose in combination. The optimal biomarker cutoff shifts the moment the standard of care it is measured against changes. The optimal price moves with competitor entry. The optimal trial size depends on the true effect size, which is the very thing you do not yet know. You are therefore not estimating a hidden-but-stationary target from sparse, biased, time-lagged data - you are tracking a target that drifts as the surrounding profile evolves. A perfect estimate can be stale by the time you act on it.

#### The coupling, and the real shape of the problem

There is a final turn that makes the picture honest. These optima are not independent. They share axes - are coupled. Dose couples to the combination. The cutoff couples to the label breadth. Price couples to access. And nearly everything couples to the comparator - which is itself a moving target, advancing as the field does. So the real object is not a tidy list of one-dimensional sweet spots; it is a **high-dimensional response surface with a non-stationary peak, observable only through expensive, ethically constrained, time-lagged, surrogate measurements that preferentially illuminate the dimensions you would rather avoid.** That sentence is the intrinsic difficulty of oncology R&D, and we haven't even talked about about decision-making latency or organizational design.

#### What this means for "productivity"

The long, well-documented decline in output per dollar - the inversion of Moore's law sometimes called Eroom's law - is usually attributed to regulatory burden, to risk-averse management, and to what the literature memorably named the "better than the Beatles" problem: every new therapy must beat an accumulating back-catalogue of effective generics. All of these are real contributors. But beneath them sits a floor that is structural rather than behavioral. In oncology, the answers we need most aren't "as much as possible" - they're "just the right amount," they're tangled up with one another, and they keep changing. Working faster doesn't fix that. What actually moves the needle is going after the hard part directly: studies that test lower doses to find the real sweet spot rather than just the highest tolerable one; sharper tests for choosing the right patients; lab and computer models that give an early read on long-term benefit; and trials nimble enough to adjust as the best answer moves.

#### What follows

If the difficulty is geometric, the response should be too. Three implications follow directly.

Treat the interior-optimum parameters as things you **continuously re-estimate**, not things you decide once. The one-dimension questions - is it potent, is it safe enough, is it differentiated — are decisions. The constrained ones - how much, for whom, how broad, with what, at what price - are running estimates that should carry an explicit confidence and a plan for which phase will sharpen them.

Invest disproportionately in the experiments that **map a down-slope.** Because a peak can only be found by characterizing both arms, the single most valuable experiment is usually the counterintuitive, expensive one that deliberately explores the worse side - randomized dose-ranging rather than another single-arm confirmation, cutoff cohorts rather than one enriched population, mono-versus-combination arms rather than an assumption. The instinct to avoid the bad side is exactly what leaves the optimum unfound.

And never optimize one diamond in isolation. Because the optima are coupled, re-checking the peak after any change to a connected axis - a new comparator, a combination, a different population - is not diligence theatre; it is the recognition that the peak you found may already have moved.

None of this makes oncology R&D easy. The point of this piece is the opposite: to be clear-eyed that a large share of the difficulty is intrinsic and will surely survive every operational improvement we can imagine. The programs that succeed are rarely the ones with the most striking biology. They are the ones whose teams located the Goldilocks points fastest, with the least self-deception about how much of each one they had actually mapped - and who kept re-locating them as the molecule reveals itself progressively in the clinic.
