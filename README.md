I came to know about QRISE 2024 on 10 March, 2024.

Link to [challenge repo](https://github.com/quantumcoalition/qrise2024-classiq-challenge).

Link to research paper titled [Exponential Quantum Speedup in Simulating Coupled Classical Oscillators](https://journals.aps.org/prx/pdf/10.1103/PhysRevX.13.041041) 📄

### Reading and Learning 📚
#### Research Paper Reading 📖

- Started reading the paper from the first day I saw QRISE 2024 on Quantum Coalition website. (Thanks YouTuber @NatashiaKaurRaina for listing all the Quantum Hackathons).
- Couldn't understand it in even second reading. 😓
- The final third reading was finished in 3rd week. 🚀

#### Watching the Research Paper Presentations 👀

- Watched the presentation by Robin Kothari (Google) from the first week. It took lots of 10-second skips backward 🙃
- Then watched the presentation by Rolando Somma (Google) in second week. It was relatively easy this time.
- Then after grasping almost all concepts, I rewatched the Robin Kothari's presentation. 📺

#### Reading Classiq Documentations 📑

- Started skimming from the 2nd week.
- Watched some tutorials from @ClassiqTechnologies and [@QWorld19](https://www.youtube.com/watch?v=4pRpX1jz6r8) (or @EducatorsMinds) YouTube channels.
- Read some more documentations. 

🔥 When I watched Nir Minerbi's [video](https://www.youtube.com/watch?v=hi-ThE-x_ko) I got to know what a astonishing work Classiq is doing! 👏🏻

### Actual Implementation 💻

- I thought to implement by creating the Initial State using raw matrices for mass, initial position, initial velocity and spring constant, which was assumed to be given in paper with some constraints.
- But I got stuck on finding the matrix $B$ from the force matrix $F$. 
- I thought, once I get matrix $H$, to implement it using the same concepts as used in [qpe-for-matrix](https://docs.classiq.io/latest/tutorials/algorithms/qpe/qpe-for-matrix/qpe-for-matrix/) notebook in Classiq tutorials.
- But then stuck at the stage of finding `pauli_ops` which are needed for Hamiltonian simulation because of unmatched matrix dimensions. 😩

### Comment on Time Complexity ⏱️

The researchers assumed that the initial state is pre-made. But, to even create the mass matrix $M$ would take $O(N) = O(2^n)$ time which violates their speedup at first hand. ❗

### Learnings

- I got to know, at least a bit, how to actually read papers more efficiently.
- I learned how classiq library is helping in implementing algorithms effortlessly.

### Further To-Dos 📝

- I would be try to read the [paper](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.127.060503) titled "Quantum Principal Component Analysis Only Achieves an Exponential Speedup Because of Its State Preparation Assumptions" by Ewin Tang. 
- Then I am thinking to analyse techniques, if possible, to prepare the assumed state and hamiltonian in the Coupled Classical Oscillation Simulation paper. 🤔

- And then lots of implementations using classiq library.
