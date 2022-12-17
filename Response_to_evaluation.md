# Evaluation

- **Status:** In progress
- **Application Document:** https://github.com/w3f/Grants-Program/blob/master/applications/faceless.md
- **Milestone:** 2
- **Kusama Identity:** [HC8pZ53SejB9YALHn2qXea6XMFFNgxpdXhVvtF7uU5dTSqu](https://kusama.subscan.io/account/HC8pZ53SejB9YALHn2qXea6XMFFNgxpdXhVvtF7uU5dTSqu)
- **Previously successfully merged evaluation:** All by 0xCaso

| Number | Deliverable | Accepted | Link | Evaluation Notes |
| ------ | ----------- | -------- | ---- |----------------- |
| 0a. | License | <ul><li>[ ] </li></ul> | [Apache License 2.0](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery/blob/2db2b8a068f48a5beae4907188b096159427fed4/Apache%20License%202.0) | See **General Notes** |
| 0b. | Documentation | <ul><li>[ ] </li></ul> | [README.md](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery/blob/2db2b8a068f48a5beae4907188b096159427fed4/README.md) | See **General Notes** |
| 0c. | Testing Guide | <ul><li>[ ] </li></ul> | [README.md#unit-tests](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery/blob/2db2b8a068f48a5beae4907188b096159427fed4/README.md#unit-tests) | See **General Notes** |
| 0d. | Tutorial | <ul><li>[ ] </li></ul> | [README.md#tutorial](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery/blob/2db2b8a068f48a5beae4907188b096159427fed4/README.md#tutorial) | See **General Notes** |
| 1. | Client modules | <ul><li>[x] </li></ul> | [*faceless* pallet](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery/blob/2db2b8a068f48a5beae4907188b096159427fed4/faceless-substrate-node/pallets/faceless/src/lib.rs) | - |
| 2. | Benchmark | <ul><li>[ ] </li></ul> | [README.md#benchmark](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery/blob/2db2b8a068f48a5beae4907188b096159427fed4/README.md#benchmark) | See **General Notes** |
| 3. | Docker | <ul><li>[x] </li></ul> | [Dockerfile](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery/blob/2db2b8a068f48a5beae4907188b096159427fed4/Dockerfile) | - |
<br/>

## General Notes v1 - Dec 14, 2022
I easily managed to setup the local environment, also with the provided Dockerfile. However, all the existing documentation in the README file is inherent in the previous milestone. For this, I'm pointing out what should be added and fixed:

## Response: 

It turns out I forgot to upload the new frontend code we have developed for milestone 2 in my previous commits, which you can now find in the [Faceless_frontend @ cfe781e
] folder of the updated [delivery](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery). Sorry for the trouble.  
*************************

### 0a. License
This is a minor problem, but it would be better to rename the license file (Apache License 2.0) to LICENSE or LICENSE.md.

### Response:

Thanks for pointing out this problem. We have updated the license name in the updated [delivery](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery). 
*************************
### 0b. Documentation
In the README, I'd add a quick description of the added features (at least for the new pallet's functionalities).
Also, in [this](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery/blob/2db2b8a068f48a5beae4907188b096159427fed4/README.md#use-substrate-to-verify-zk-proof) section, you should change the website address from http://localhost:8000 to http://localhost:3000/substrate-front-end-template.

### Response:

Thanks for pointing out this problem. We have added the description in [here](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery#about-faceless-apis-newly-added-features), and changed the website address in [here]
(https://github.com/HeisenbergLin22/Faceless_milestone2_delivery#use-substrate-to-verify-zk-proof). 
*************************

### 0c. Testing Guide
It seems that no unit tests for the new pallet's functions have been added, correct me if I'm wrong.

### Response:

Yes, you are right. We have provided the unit tests of the underlying AIBE scheme and ZKP algorithms, but it's not clear how to carry out the unit tests for the pallet's functions as it requires some global chain configuration and input construction. Therefore, as recommended in the unit test [notes](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery#run-tests), 
we recommend the users read the [Tutorial](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery#tutorial) section on how to test the new features.
*************************

### 0d. Tutorial
In the tutorial section, I'd add a little guide that explains how to test the new features, as it hasn't been updated since the previous milestone.

### Response:
Thanks for the comments. We have added the guide [here](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery#faceless-dapp-test). 
*************************

### 2. Benchmark
You should update the benchmark section in the README file, as it hasn't been updated since the previous milestone, and there are no info about the new functions' benchmarks.

### Response:
Thanks for the comments. We have updated the [benchmark](https://github.com/HeisenbergLin22/Faceless_milestone2_delivery#benchmark) section with the benchmark results of the pallet functions. 
*************************
