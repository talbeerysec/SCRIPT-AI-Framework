# The  SCRIPT framework for AI's impact evaluation
We present the SCRIPT framework, formalized from Karpathy’s heuristic, for evaluating AI’s impact on any domain. We then apply it to the information security domain

![The SCRIPT framework](/image/The%20SCRIPT%20framework.png)




To use this SCRIPT Framework , consider the following prompt (used with Claude Sonnet 4.5) 
```
Please read https://raw.githubusercontent.com/talbeerysec/SCRIPT-AI-Framework/main/SCRIPT-context.txt for context,
then using the format of this scorecard for lateral movement for attackers in https://raw.githubusercontent.com/talbeerysec/SCRIPT-AI-Framework/refs/heads/main/Scorecards/lateral_movement_attacker_scorecard.html 
and using the format of this scorecard for lateral movement for defnders in https://raw.githubusercontent.com/talbeerysec/SCRIPT-AI-Framework/refs/heads/main/Scorecards/lateral_movement_defender_scorecard.html 
create similar scorecards for attackers and defenders for <a security domainn, e.g. Vulnerability management>

```
