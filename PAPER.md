# Constitutional Governance for AI Systems

## Why Trusting the Model Is the Wrong Problem

James A. Tillar, Tillar Technologies LLC

*Status: working paper. It sets out a theory and the reasoning behind it. It is not a report of proven results.*

## Executive Summary

Most talk about AI governance is about model behavior: better prompts, stronger guardrails, better alignment. These help performance. But a model that behaves well has not shown that an action is authorized or correct.

This paper proposes a constitutional approach: no one is trusted automatically. Models, users, administrators and architects all work through a framework that checks their authority and independently verifies each proposed action before it can touch a live system.

The model may propose an action. It must never authorize that action itself.

## 1 The Fundamental Problem

Large language models work by probability. They can misread intent, drift from their instructions, and give convincing answers that are wrong or unsupported. Better behavior matters, but it does not answer a separate question: who has permission to act?

A persuasive answer is not an authorization. A correct answer is not permission to change a system. Governance has to enforce that difference. The real question is not only whether a model can be trusted, but why its output should carry authority at all.

## 2 Governance and Behavioral Control

Prompt engineering, safety instructions, constitutional prompting and alignment tuning shape what a model produces. They do not, on their own, draw an independent boundary around what it may do.

Governance controls do a different job. Identity checks establish who is acting. Chains of authorization and limits on scope settle what that actor may do. Independent verification checks the result. Protected audit records keep the evidence.

These controls must sit outside the model's reach. A model must not be able to reinterpret a restriction, approve its own exception or rewrite the record of what it did.

## 3 The Zero Trust Governance Model

No actor is exempt from verification. A request from an administrator or the architect meets the same requirements as a request from an AI agent, even though their permitted scopes differ.

Authority attaches to a specific, verified permission, not to confidence in whoever is asking. The framework must also be protected and tested. Its policies, checks and boundaries cannot be assumed to be flawless.

## 4 Why the Architect Became Untrusted

Repeated red-team exercises (deliberate attempts to break the design) showed the architect to be a recurring point of attack. This was not necessarily because of bad intent. A person with broad authority can be persuaded, distracted, tired or rushed into approving what they would normally refuse.

If the creator can bypass the controls whenever they are inconvenient, the controls are optional. Constitutional governance requires the architect to follow the rules too.

The rules can still change. But amendments and emergency procedures must follow a defined, checkable process, not an informal override.

## 5 The Constitutional Action Lifecycle

Changes to live systems follow eight steps. Permission to try a change in isolation is separate from permission to release its result.

1. **Identity.** The actor proves who they are before asking for anything.
2. **Intent declaration.** The request states what will change, why, and what result is expected.
3. **Authorization.** The request is checked against the actor's permissions, the applicable policy and the approved scope.
4. **Temporary permission.** A narrow permission is issued for this action and a limited time.
5. **Sandbox execution.** The action runs in isolation. The requesting actor has no direct access to the live system by this route.
6. **Validation and testing.** Independent checks measure the result against set requirements.
7. **Intent reconciliation.** What actually happened is compared with the declared intent, the approved scope and the expected result.
8. **Production promotion.** Only a result that passes the required checks may move to the live system, through a controlled path.

Some operations cannot be staged like a software change. For those, the system must define an equivalent controlled boundary, and the permission must say what may happen before any irreversible effect.

## 6 AI as an Untrusted Actor

AI gets no special exemption. It must prove its identity, declare its intent, request permission, and show evidence that it stayed in scope. It cannot grant itself authority, widen its permissions or approve its own changes.

If a required condition is missing or fails verification, the action is rejected and the reason is recorded. A warning that still lets the action proceed does not enforce the boundary.

## 7 Governance as Models Become More Capable

The framework does not depend on settling whether future models become emotional, strategic or more autonomous. A more capable model still has to meet the requirements for identity, authorization, scope and evidence.

Those requirements stay in force as models change. Their enforcement must keep being tested against stronger attempts to get around them. More capability is not a reason to relax the boundary.

## 8 Constitutional Principles

1. Authority is external to the model.
2. Evidence supports a decision but does not itself grant authorization.
3. Intent must be declared before permission is issued.
4. Every governed action must produce evidence that can be independently checked.
5. No actor may expand their own authority.
6. Production promotion follows verification.
7. No actor receives implicit trust or an exemption from the governing process.

## 9 Implications for High Consequence AI

This approach is meant for settings where a wrong or unauthorized action can have serious consequences: government, healthcare, biotechnology, scientific research, critical infrastructure, software delivery and autonomous operations.

Each setting must define its own acceptable evidence and release conditions. A passed test shows only what that test can show. The framework must keep those limits visible and not treat one successful check as proof of universal correctness.

## Conclusion

Reliable AI governance cannot rest on hoping that the model, or the person directing it, will always behave. It needs enforceable rules about which actions are allowed and what evidence is required before results reach production.

Models may propose. Governance decides. Authority comes from the governing process, not from an actor's confidence, status or skill at persuading.
