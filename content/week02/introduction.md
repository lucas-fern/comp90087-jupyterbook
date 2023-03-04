# Summary

## Contractual Trust
Contractual trust
: Humans trusting a machine to fulfil a **contract** in a particular **context**

### Trust, Distrust, and Lack of Trust

#### Trust
A *trusts* B if:
- A believes that B will act in A's best interests; and
- A accepts vulnerability to B's actions; so that:
- A can anticipate the impact of B's actions, enabling collaboration.

#### Distrust
A *distrusts* B if:
- A believes B will act *against* A's best interests.

#### Lack of Trust
A *lacks trust in* B if either of the following is true:
- A does *not* believe that B will act in A's best interests; or
- A does *not* accept vulnerability to B's actions.

Lack of trust simply requires an *absence of trust*, where **distrust** instead requires A to believe B will act *against* A's interests. 

### Contracts for AI
```{figure} ../../images/contracts-in-trust.png
:name: contracts-in-trust

The set of contracts that a AI should uphold to be considered trustworthy according to European guidelines. Source: [Formalizing Trust in Artificial Intelligence: Prerequisites, Causes and Goals of Human Trust in AI](https://arxiv.org/abs/2010.07487)
```

### Warranted and Unwarranted Trust
<table>
<tbody>
  <tr>
    <td></td>
    <td><b>Trusted</b></td>
    <td><b>Distrusted</b></td>
  </tr>
  <tr>
    <td><b>Trustworthy</b></td>
    <td>Warranted Trust</td>
    <td>Unwarranted Distrust</td>
  </tr>
  <tr>
    <td><b>Not Trustworthy</b></td>
    <td>Unwarranted Trust</td>
    <td>Warranted Distrust</td>
  </tr>
</tbody>
</table>

### Use, Misuse, Disuse, and Abuse of Automation

#### Misuse
Using automation where it *shouldn't* be used.

Caused by:
```{toggle}
Unwarranted Trust
```

#### Disuse
Not using automation when it *should* be used.

Caused by:
```{toggle}
Unwarranted Distrust
```

#### Abuse
***Deploying*** automation where it *shouldn't* be deployed.

Caused by:
```{toggle}
Unwarranted Distrust on the part of the AI designer.

Can arise if:
- the AI designer has (unwarranted) distrust in human operators,
    - believes their AI solution will be better (unwarranted trust in their AI).
- designers or decision makers are biased in favour of automation,
- designers or decision makers are arrogant.
```

## Power
Power
: The ability to control our circumstances

### User Control
```{figure} ../../images/ethical-user-trust.png
:name: ethical-user-trust

An ethical relationship between a user and machine, where the user has the *power* to disengage if distrust is established.
```

```{figure} ../../images/unethical-user-trust.png
:name: unethical-user-trust

An unethical power relationship between a user (decision subject), decision maker, and machine; where the user distrusts the machine, the decision maker has the power to enforce it's use, and the decision maker is not vulnerable to negative consequences that arise from the machine's decisions.
```