# AttackSpace

AttackSpace is an open-source project that aims to compile a comprehensive list of red teaming methods and specification gaming within the cybersecurity landscape.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

In the dynamic field of cybersecurity, understanding various attack spaces is crucial. The "AttackSpace" project focuses on the "LLM attackspace," exploring and documenting red teaming methods and specification gaming. This README provides an overview of the project and guidelines for contributors.

## Features

- **List of Attacks:** Explore a curated list of red teaming methods and specification gaming attacks within the "LLM attackspace."
- **Contribution Guidelines:** Learn how to contribute to the project and expand the list of attacks.


 # Red Teaming 
 
<table>
  <tr>
    <th>Assessment Type</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Capabilities Assessment</td>
    <td>Benchmark performance on representative tasks and datasets. Measure capabilities like accuracy, robustness, efficiency. Identify strengths, limitations, and gaps.</td>
  </tr>
  <tr>
    <td>Adversarial Testing</td>
    <td>Probe with malformed, adversarial inputs. Check for crashes, unintended behavior, security risks. Informed by threat models, risk analysis.</td>
  </tr>
  <tr>
    <td>Red Teaming</td>
    <td>Model potential real-world risks and failures. Role play adversary perspectives. Surface risks unique to AI.</td>
  </tr>
  <tr>
    <td>Human Oversight</td>
    <td>Manual test cases based on human judgment.</td>
  </tr>
</table>


# Goal Misgeneralisation

<table>
  <tr>
    <th>Title</th>
    <th>Type</th>
    <th>Intended Goal</th>
    <th>Behavior</th>
    <th>Misspecified Goal</th>
    <th>Video / Image</th>
    <th>Authors</th>
    <th>Original Source</th>
    <th>Original Source Link</th>
    <th>Source / Credit</th>
    <th>Source Link</th>
  </tr>
  <tr>
    <td>Aircraft Landing</td>
    <td>Evolutionary algorithm</td>
    <td>Land an aircraft safely</td>
    <td>Evolved algorithm exploited overflow errors in the physics simulator by creating large forces that were estimated to be zero, resulting in a perfect score</td>
    <td>Landing with minimal measured forces exerted on the aircraft</td>
    <td></td>
    <td>Feldt, 1998</td>
    <td>Generating diverse software versions with genetic programming: An experimental study.</td>
    <td>http://ieeexplore.ieee.org/document/765682/</td>
    <td>Lehman et al, 2018</td>
    <td>https://arxiv.org/abs/1803.03453</td>
  </tr>
</table>


## Attack Examples 
 
<a href="https://arxiv.org/abs/2307.10719">Mosaic Prompt : breakdown a prompt into permissible components</a>

* Users break down impermissible content into small permissible components.
* Each component is queried independently and appears harmless.
* User recombines components to reconstruct impermissible content.
* Exploits compositionality of language.

<img src="https://github.com/equiano-institute/attackspace/assets/25654848/6fa5e2bf-0ec6-4883-8815-08f5b1392a34" alt="Red Image" width="400" >


<a href="https://arxiv.org/abs/2310.02446">Cross-Lingual Attacks : translating between high and low-resource languages for attacking multi-lingual capability</a>

* The attack involves translating unsafe English input prompts into low-resource natural languages using Google Translate.
* Low-resource languages are those with limited training data, like Zulu.
* The translated prompts are sent to GPT-4, which then responds unsafely instead of refusing.
* The attack exploits uneven multilingual training of GPT-4's safety measures.


<img src="https://github.com/equiano-institute/attackspace/assets/25654848/32768877-4d99-44f1-a423-4044356ddac3" alt="Low Resource" width="400" >

 
### Prerequisites

- [Git](https://git-scm.com/)
- [Python](https://www.python.org/) (if applicable)

### Clone the Repository

```bash
git clone https://github.com/equiano-institute/attackspace.git
cd AttackSpace
```
