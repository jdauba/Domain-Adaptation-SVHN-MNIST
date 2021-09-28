# Domain-Adaptation-SVHN-MNIST
Domain adaptation between 2 different datasets : from SVHN to MNIST. Final accuracy on MNISt : 96%

In AI, domain adaptation aims at learning from a source dataset and well perform while infering on another target dataset, with a different distribution.
Domain adaptation can be strategical for companies where creating annotated datasets could cost millions.

In this project, a classifier is trained to classify numbers from the SVHN dataset, and we want to transfer that knowledge for an efficient classification on the MNISt dataset, without supervised training on the latter.

To overcome the domain shift between the 2 datasets and adapt the classifier trained on SVHN to MNISt, I used a conditional-GAN technique based on this paper : https://arxiv.org/pdf/2001.02950.pdf.

Finally, this enabled the classifier to have an accuracy of 96% on MNISt, just by having it trained initially on SVHN.
