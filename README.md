# ZoKrates DevEase

## Vision
Make ZoKrates more powerful with Decision Tree Prediction(ZoKrates-DTP) and Pedersen Commitment. 

## Description
ZoKrates is a vital toolset and language for developing and verifying zk-SNARKs (Zero-Knowledge Succinct Non-Interactive Argument of Knowledge), a groundbreaking cryptographic technology that ensures privacy and scalability in various blockchain applications. As the demand for secure and efficient decentralized systems grows, ZoKrates plays a crucial role in enabling developers to create privacy-preserving protocols.

However, the current state of ZoKrates presents challenges that hinder its full potential. The ZoKrates DevEase aims to address these challenges by bring machine learning abilities, enhancing the existing libraries, and providing the up-to-date tutorial. This initiative is not only essential for the growth of ZoKrates but also pivotal in advancing the broader field of cryptography and decentralized technology.

## Goals
Bring in machine learning abilities: Develop the Zero Knowledge Decision Tree Prediction for ZoKrates (ZoKrates-DTP), which could directly translate the decision tree with python to ZoKrates.

Integrate new libraries: Integrate the Pedersen Commitment scheme to the whole ZoKrates DevEase project and set the plan for Type Conversions libraries.

Enhance Official Documentation and Tutorials: Revamp and update the existing documentation to make it more accurate, informative, and user-friendly, with a particular focus on the ether.js and standard library.

## Plans

```plantuml
------------------------------
|   ZoKrates DevEase         |
------------------------------
| -[x] ZoKrates-DTP          |
| -[x] Pedersen Commitment   |
| -[x] Tutorial for ether.js |
------------------------------
```
The main accomplishments of this hackathon include: ZoKrates-DTP is implemented with reference to ZK-DTP, the main code is in ./Decision Tree Prediction/plot_iris_dtc.ipynb and ./Decision Tree Prediction/Demo. In addition an integration of Pedersen Commitment has been made. In the tutorial I wrote how to use ether.js to call EVM contracts to verify ZoKrates proofs. The official documentation for this part is outdated and can be very misleading for developers.

### TODO: Streamlined Perceptron Library for Neural Network Builders
Recognizing the significance of neural networks in machine learning, our project introduces a streamlined Perceptron library. This library simplifies the integration of Perceptron, a fundamental building block in neural networks, into ZoKrates. By providing developers with easy-to-use tools, we empower them to construct and train advanced neural networks, harnessing the potential of zero-knowledge methodologies to preserve privacy and confidentiality.


## Summary
Our project marks a good milestone in the advancement of zero-knowledge computation on ZoKrates. By combining the Decision Tree Prediction(ZoKrates-DTP) and Pedersen Commitment, we offer developers the means to build privacy-preserving and secure ML applications. Our project is not an end, but the beginning of strengthening ZoKrates capabilities and developer-friendliness in extensions and integrations.

## Demo
- [Decision Tree Prediction(ZoKrates-DTP)](https://www.youtube.com/watch?v=jCn-xm2Amoo)
- [Pedersen Commitment Library](https://youtu.be/8kZHOQtp1Ck)


Join us on this transformative journey as we empower developers to unlock the full potential of zero-knowledge proof, fostering privacy, security, and trust on the Moonbeam network. 

*Notes: This project is based on ZoKrates and ZK-DTP. We also maintain a [Buidl at Dorahacks](https://dorahacks.io/buidl/7000)*