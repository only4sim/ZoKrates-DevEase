# ZoKrates DevEase

## Vision
Make ZoKrates more powerful and user-friendly.

## Description
ZoKrates is a vital toolset and language for developing and verifying zk-SNARKs (Zero-Knowledge Succinct Non-Interactive Argument of Knowledge), a groundbreaking cryptographic technology that ensures privacy and scalability in various blockchain applications. As the demand for secure and efficient decentralized systems grows, ZoKrates plays a crucial role in enabling developers to create privacy-preserving protocols.

However, the current state of ZoKrates presents challenges that hinder its full potential. The ZoKrates Library Extensions and Developer-Friendliness Improvements project aims to address these challenges by enhancing the existing libraries, simplifying development processes, and providing comprehensive documentation. This initiative is not only essential for the growth of ZoKrates but also pivotal in advancing the broader field of cryptography and decentralized technology.


## Importance of the Project
Enhancing Functionality: Expanding the common libraries with different commitment schemes and type conversions will provide developers with more tools, enhancing the functionality and versatility of ZoKrates.

Simplifying Development: The introduction of an ether.js library will streamline the development process, making ZoKrates more approachable and reducing the learning curve for new developers.

Improving Documentation: Comprehensive and accurate documentation is vital for developer efficiency and innovation. By improving the official documentation and tutorials, this project will foster a more informed and collaborative community.

## Goals
Expand Common Libraries: Introduce additional commitment schemes, type conversions, and other essential components to enrich the ZoKrates library.

Simplify Development with ether.js Library: Develop an ether.js library to streamline ZoKrates development, replacing the current defunct Javascript call instructions.

Enhance Official Documentation and Tutorials: Revamp and update the existing documentation to make it more accurate, informative, and user-friendly, with a particular focus on the standard library.

## Plans
### Expand Common Libraries

- Assessment of Current Libraries: Analyze existing libraries to identify gaps and areas for expansion.

- Development of Commitment Schemes: Implement various commitment schemes to enhance security and functionality.

- Type Conversions: Create a robust set of type conversion functions to facilitate seamless development.

### Simplify Development with ether.js Library

- Analysis of Current Javascript Instructions: Identify the limitations and issues with the existing Javascript call instructions.

- Development of ether.js Library: Design and implement an ether.js library tailored to ZoKrates, ensuring compatibility and ease of use.

### Enhance Official Documentation and Tutorials

- Audit of Existing Documentation: Conduct a thorough review of the current documentation to pinpoint inaccuracies and areas for improvement.

- Update Standard Library Information: Provide detailed information about the standard library, including examples and best practices.

- Creation of New Tutorials: Develop comprehensive tutorials that guide developers through various aspects of ZoKrates development.

### 

```plantuml
---------------------------
|   ZoKrates DevEase       |
---------------------------
| -[x] Zokrates Connector  |
| -[x] Pedersen Commitment |
| -[]  Others             |
----------------------------
```

### Overcoming Verification Challenges
A key contribution of our project is tackling the persistent verification issues related to data types in on-chain processes. We recognize the paramount importance of efficient and reliable data verification for ensuring the integrity and validity of machine learning models. By harnessing the capabilities of Zokrates, we empower developers and researchers to overcome these challenges, facilitating trustworthy machine learning applications on Moonbeam. In addition, we have also solved the type matching problem of Zokrates when using ether.js, which is incorrectly documented in the current Zokrates documentation.

### Robust Pedersen Commitment Library
To enhance privacy and confidentiality in zero-knowledge machine learning, we have developed a robust Pedersen commitment library. Pedersen commitments play a crucial role in securely masking and encrypting sensitive data inputs within machine learning models. Our user-friendly and comprehensive library allows developers to seamlessly integrate this cryptographic technique into their Moonbeam applications, bolstering data privacy and enabling secure training and inference.

### TODO: Streamlined Perceptron Library for Neural Network Builders
Recognizing the significance of neural networks in machine learning, our project introduces a streamlined Perceptron library. This library simplifies the integration of Perceptron, a fundamental building block in neural networks, into Moonbeam. By providing developers with easy-to-use tools, we empower them to construct and train advanced neural networks, harnessing the potential of zero-knowledge methodologies to preserve privacy and confidentiality.


### Summary
Our project marks a good milestone in the advancement of zero-knowledge computation on Moonbeam. By combining the power of Zokrates with essential libraries, we offer developers the means to build privacy-preserving and secure applications. Whether it's overcoming verification challenges, leveraging Pedersen commitments for data masking, or utilizing the Perceptron library for neural network builders, our project sets the stage for the future of zero-knowledge computation on the Moonbeam blockchain.

### Demo
- [Pedersen Commitment Library](https://youtu.be/8kZHOQtp1Ck)


Join us on this transformative journey as we empower developers to unlock the full potential of zero-knowledge proof, fostering privacy, security, and trust on the Moonbeam network. 

*Notes: This project is based on ZoKrates and zk-base-Moonbeam and has been reorganized for JS calls. We also maintain a [Buidl at Dorahacks](https://dorahacks.io/buidl/7000)*