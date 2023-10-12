# RL_snakegame
 AI agent for a snake game from FreeCampCode tutorial : https://www.youtube.com/watch?v=L8ypSXwyBds&t=1795s


Update on Snake Game Reinforcement Learning Model

Adjusted Reward Structure:

In my continuous endeavor to optimize the behavior of the snake in the game, I've refined the reward system for the reinforcement learning model. The adjusted rewards aim to more accurately guide the agent towards better decision-making and game performance. Here's a breakdown:

Collision Penalty : -10
To strongly dissuade the agent from crashing into the walls or itself, a substantial penalty has been introduced for any collisions.
Consuming Food Reward : +10
To emphasize the main goal of the game, I provide a significant reward for every food item consumed.
Getting Closer to Food Reward : +0.05
To promote a more proactive approach towards the target, a small reward is given when the snake moves closer to the food item.
Moving Away from Food Penalty : -0.05
To discourage wasteful moves, a penalty is introduced if the snake increases its distance from the food.
Iteration Penalty : -1
To discourage aimless wandering and encourage swift, purposeful movement, a small penalty is applied for every game iteration.


Transition to LSTM:
After carefully analyzing the current model's behavior and performance, I'm considering transitioning to a Long Short-Term Memory (LSTM) based model for the snake game. LSTMs are a type of recurrent neural network (RNN) that can remember patterns over long sequences. They are particularly well-suited for problems where the agent needs to remember past actions or states to make informed decisions.

For the snake game, the ability to 'recall' past moves can potentially help the snake avoid circular patterns and make better strategic decisions regarding food consumption. As the snake grows, it becomes increasingly crucial for it to be aware of its tail's position and the spaces it has previously occupied. By employing LSTMs, I hope to capture this temporal aspect of the game and thereby improve the agent's efficiency and intelligence.
