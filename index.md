# SwiftGuard-Website

## Introduction

  Large language models (LLMs), such as ChatGPT, are increasingly deployed across industries, from healthcare to finance. Despite their widespread utility, these models remain vulnerable to jailbreaking attacks that evade safety guardrails to generate objectionable content upon the request of a user with mal-intent. This vulnerability undermines trust and limits LLM deployment in sensitive domains.

<center>
<details>
<summary><span style="color:blue">Our Antagonist</span></summary>
<br>
  PAIR (Prompt Automatic Iterative Response) uses recursivity and prompt-based jailbreaking to get around the embedded safeguards that are present in LLMs. Prompt-based jailbreaking is a social-engineering based strategy in which certain techniques are used to change the semantics or context of a malicious prompt to make it appear safer to the LLM. Prior to algorithms like PAIR, these jailbreaks were created purely by humans. PAIR introduces an automatic approach that is meant to jailbreak LLMs with little-to-no human involvement.
</details>
</center>

<center>
<details>
<summary><span style="color:blue">Our "Imperfect" Protagonist</span></summary>
<br>
  SemanticSmooth, a recently invented LLM defense, mitigates PAIR's tactics by employing semantic perturbations and aggregating predictions to detect and then deny adversarial attacks. However, its reliance on reinforcement learning introduces significant computational overhead and performance trade-offs, particularly for benign prompts. The excessive installation of this defense significantly slows down the process, especially for the strong majority of LLM users who only pose benign prompts.
</details>
</center>

<center>
<details>
<summary><span style="color:blue">Our "Perfected" Protagonist</span></summary>
<br>
  Addressing this runtime inefficiency is critical for ensuring that defending LLMs can be both robust (as it relates to detecting adversarial prompts) and computationally efficient (for all kinds of prompts). Our proposal focuses on replacing SemanticSmooth's reinforcement learning component with an algorithmic framework that does not rely on an ever-changing policy network. This framework will identify attacks based on detectable semantic perturbations and selectively apply appropriate transformations. This method not only preserves SemanticSmooth's robustness but enhances efficiency in regard to average response time. Preliminary research from PAIR and SemanticSmooth papers suggests that certain semantic transformations (e.g., summarization or paraphrasing) can reveal attacks without significant computational penalties, hence being dubbed "SwiftGuard".
</details>
</center>

## Methods
  Determining how effective of an approach SwiftGuard is requires testing it on numerous prompts which we have collected and categorized into three distinct groups:
  
![alt text](/images/sg_pipeline.png “The SwiftGuard Pipeline”)

## Results

## Conclusion

### Our group
[Donald Taggart](https://www.example.com) [Arman Rahman](https://www.example.com) [Shreya Sudan](https://www.example.com) [Dante Testini](https://www.example.com)
### would like to thank our mentors
[Barna Saha (Mentor)](https://barnasaha.net/) [Arya Mazumdar (Mentor)](https://mazumdar.ucsd.edu/)
