

# Poker Hand Detector - Real-time Poker Hands Recognition using YOLOv8 Object Detection






## Introduction

Poker Hand Detector is a Python-based project that utilizes YOLOv8, an efficient object detection model, to recognize and classify poker hands from images or videos. The project aims to facilitate real-time hand recognition for various applications, such as poker game assistance or hand analysis during gameplay.

## About Poker Hand Game
In the game of poker, players are dealt a combination of five playing cards from a standard deck of 52 cards. The objective is to form the best possible hand based on the established poker hand rankings. The rank of a poker hand determines its strength, and at the showdown, the player with the highest-ranking hand wins the pot.

### List of Poker Hands (In Descending Order of Strength)

1. #### Royal Flush: 
A hand containing the five highest-ranking cards of the same suit (Ace, King, Queen, Jack, and Ten).

2. #### Straight Flush: 
Five consecutive cards of the same suit.

3. #### Four of a Kind: 
Four cards of the same rank, accompanied by any fifth card (known as the "kicker").

4. #### Full House: 
Three cards of one rank and two cards of another rank.

5. #### Flush: 
Five cards of the same suit, not in consecutive order.

6. #### Straight: 
Five consecutive cards of any suit.

7. #### Three of a Kind: 
Three cards of the same rank, accompanied by two unrelated cards.

8. #### Two Pair: 
Two sets of two cards of the same rank, accompanied by any fifth card.

9. #### One Pair: 
Two cards of the same rank, accompanied by three unrelated cards.

10. #### High Card: 
When no player forms any of the above hands, the highest-ranking card in their hand determines the winner. If two players have the same high card, the second-highest card, and so on, are used to determine the winner.



![game](https://github.com/ishita126jain/Poker-Hand-Detector/assets/91709949/eb75e7f6-3b6a-4587-8d94-22ede9cd4133)
## Prerequisites

- Python 3.6 or higher

- [Virtualenv](https://virtualenv.pypa.io/en/latest/) (optional but recommended)

## Installation

1. Create a virtual environment and activate it:

```bash
virtualenv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
```
2. Install required packages:
```bash
pip install -r requirements.txt
```
## Training the Model
1. Download YOLOv8 model from Roboflow:

- Download the YOLOv8 model file from [Roboflow](https://universe.roboflow.com/) and place it in the weights/ directory.

2. Train the model on Google Colab:

- Follow the steps outlined in the colab file (Yolov8.ipynb) to train the model using your custom dataset.
  
## Usage

1. Prepare your video:

- Place your video file in the project directory. Or start your webcame


2. Run the Poker Hand Detector:
```bash
python Poker-hand-detector.py 
``` 

3. View the results:

- The processed video with Poker Hand Detector will identifies cards and lable there ranks and suits and if there is exactly five cards in a hand then detect the type of hand.


## Configuration
- You can customize the confidence threshold for Poker hand detection by modifying the conf parameter in Poker=Hand-Detector.py. The default value is set to 0.5.
## Acknowledgements

 - [Ultralytics](https://github.com/ultralytics/ultralytics)
 - [CVzone library by CVzone](https://github.com/cvzone/cvzone)
 


## Contribution

Contributions are always welcome!

If you find any issues or have suggestions for improvements, feel free to create a pull request.


## Contact
For any questions or inquiries, please contact us at [ishita126jain@gmail.com](ishita126jain@gmail.com).
