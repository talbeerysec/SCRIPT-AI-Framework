# The SCRIPT Framework for AI's Impact Evaluation

The SCRIPT framework evaluates how AI automation affects different tasks and domains. Formalized from [Andrej Karpathy's heuristic](https://twitter.com/karpathy/status/1850600302727913768), it reveals why AI provides attackers a structural advantage over defenders in information security.

![The SCRIPT framework](/image/The%20SCRIPT%20framework.png)

## What is SCRIPT?

**S**hort: Brief in time  
**C**losed: Requires limited context  
**R**epetitive: Repetition of one rote task  
**I**ndependent: Standalone  
**P**ermissive: Forgiving of mistakes  
**T**ech-ready: Digitally automatable

Tasks scoring high on SCRIPT (15-18/18) are ideal candidates for AI automation. Tasks scoring low (0-9/18) require human expertise and judgment.

## Scoring Guide

Each SCRIPT dimension is scored 0-3:
- **0** = Not at all
- **1** = Somewhat  
- **2** = Mostly
- **3** = Completely

**Total Score Range:** 0-18 points

## Example Scorecards

### Information Security Use Cases

| Domain | Attacker Score | Defender Score | Gap |
|--------|---------------|----------------|-----|
| [Lateral Movement](Scorecards/) | 18/18 ⭐⭐⭐⭐⭐ | 8/18 ⭐⭐ | +10 |
| [Phishing](Scorecards/) | 18/18 ⭐⭐⭐⭐⭐ | 12/18 ⭐⭐⭐ | +6 |
| [Vulnerability Management](Scorecards/) | 18/18 ⭐⭐⭐⭐⭐ | 13/18 ⭐⭐⭐⭐ | +5 |

**Key Insight:** Attackers consistently score perfect 18/18 because their tasks are repetitive, error-tolerant, brief, context-light, and independent. Defenders struggle with context requirements and error intolerance.

## Create Your Own Scorecards

Use this prompt with Claude Sonnet 4.5 to evaluate any security domain:
```
Please read https://raw.githubusercontent.com/talbeerysec/SCRIPT-AI-Framework/main/SCRIPT-context.txt for context,
then using the format of this scorecard for lateral movement for attackers in https://raw.githubusercontent.com/talbeerysec/SCRIPT-AI-Framework/refs/heads/main/Scorecards/lateral_movement_attacker_scorecard.html 
and using the format of this scorecard for lateral movement for defenders in https://raw.githubusercontent.com/talbeerysec/SCRIPT-AI-Framework/refs/heads/main/Scorecards/lateral_movement_defender_scorecard.html 
create similar scorecards for attackers and defenders for <your security domain, e.g., Incident Response, Threat Hunting, etc.>
```

Replace `<your security domain>` with your specific use case.

## Repository Contents

- **`/Scorecards/`** - Interactive HTML scorecards for various security domains
- **`SCRIPT-context.txt`** - Full framework definition and scoring guidelines
- **`/image/`** - Framework diagrams and visualizations

## Background

**Read the full analysis:**  
📝 [Follow the SCRIPT: Why Attackers are Winning the AI Arms Race](https://medium.com/@TalBeerySec/follow-the-script-why-attackers-are-winning-the-ai-arms-race-39de80748d09)

**The Two Dimensions:**
1. **Automation Readiness** (R, P, T): Is this task suitable for automation at all?
2. **Context Window Fit** (S, C, I): Can this fit in an AI's limited memory?


## Acknowledgements

Claude Sonnet 4.5 for scorecard generation and analysis.

## License

[Your License Here]
