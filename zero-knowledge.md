# Session 1  Introduction to ZK

![image-20230221233556331](https://github.com/shiyivei/zero-knowledge/blob/main/images/session1_brain_map.png)

## 1.1 Why ZK

1. ZK crypto is more important and general (expecially for arbitrary computing, etc)
2. ZK crypto is easier to use and make contributions (not as difficult as we imagined)
3. ZK crypto is fun and challenging (more potential rewards and creative answers of tough questions)

## 1.2 About Course

1. Theory of modern ZK crypto
2. Toolstacks and usage
3. Applications and design patterns

## 1.3 Logistics 

1. Time
2. Communication channel: Discord
3. Resources:zkiap.com
4. Office hour
5. Promble sets
6. Projects: active in program and buidling examples
7. PLONKathon （）

## 1.4 Pre-requisites

1. Number theory and group theory

2. Cryptographic primitives

3. Algebraic concepts,esp,polynomials

## 1.5 ZK Proofs/Protocols

1. concept:  prove sth to sb instead of telling
2. three properties: zk （don't reveal underlying info）; Completeness (can answer anything about underlying info); Soundness （if cheat, will get caught ）

3. examples: digital signature
4. zkps are old: there are some applications and questions

## 1.6 Exercises

### **1.6.1 ZKP for 3-coloring Demo**

**Q1 :** Currently, you can only select adjacent pairs of nodes to check. Would the proof still be zero knowledge if you could pick arbitrary pairs of nodes to check?

**A1 :** If I can pick arbitrary pairs of nodes to check, it means I can infer all the underlying information (the color of the whole graph) based on the two nodes, that is no longer a zero-knowledge proof

**Q2:** The equation currently being used for confidence is `1-(1/E)^n`, where `E` is the number of edges in the graph, and `n` is the number of trials run. Is this the correct equation? Why is there no prior?

**A2:**  It's correct, as the number of trials increases (that is, the more questions the experimenter asks), the more certain the statement is true (`1-(1/E)^n` => 100% sure)

### **1.6.2 Optional - ZKP for DLOG**

I Have not finished yet，hard working...

### **1.6.3 zkmessage.xyz**

**Q1 :** Explain why you need to generate and save a “secret” value

**A1 :** secret it the tool that I can use to proof sth. It's unique

**Q2 :** Write out a plain-English explanation of what statement is being proven in ZK

**A2:** It can be any fact that the prover can prove, such as someone who says to hold a certain encrypted account, he can prove his statement is true by paying a transfer

**Q3 :** Log into the same zkmessage account, from a different browser or computer. Explain why zkmessage can’t just use a simple “username/password” system like most social apps.

**A3:** In fact, many encryption schemes used by zero-knowledge have good collision resistance (it is almost impossible to derive passwords from user name in probability), but account password schemes used by social applications are easy to guess passwords through calculations

# Session 3  Mathematical building blocks

## 3.1 formalization of zero-knowledge

## 3.2 discrete logarithm

## 3.3 common cryptographic sources of “hardness,” 

## 3.4 elliptic curve cryptography

## 3.5 pairing-based cryptography