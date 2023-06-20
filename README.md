# TIM-TOM

TIM-TOM is a custom Deep SARSA Reinforcement Learning Agent currently in development for trading options on the Forex market. TIM-TOM consists of sub-agents, each powered by a custom deep learning architecture, working together to reach optimal action policies and maximize targets. These sub-agents interact in a custom environment, earning diverse trading policies through competition and cooperation, all aimed at achieving maximized targets.

The decision policies in the current state of TIM-TOM encompass six action calls:

(1) Open a buy.
(2) Open a sell.
(3) Close the first open buy.
(4) Close the first open sell.
(5) Hold.
(6) Close all positions.


With this range of action calls and a customized position sizing strategy, the agent learns to interact effectively with its environment. We employ an optimization method that allows TIM-TOM to tune towards optimal decision policies for positive target outputs.

This cutting-edge AI technology is designed to analyze and predict market trends swiftly and accurately, empowering the agents to make intelligent investing decisions and maximize returns. TIM-TOM, equipped with its powerful custom deep learning networks, demonstrates promising potential in identifying profitable trading opportunities. It exhibits the capability to execute trades with remarkable speed, precision, and consideration for associated fees. Furthermore, TIM-TOM is developed to enhance stability in the learned trading schemes, allowing for improved generalization over time and synchronization with a better risk and reward framework to achieve optimal target outputs.

Presently, TIM-TOM is in the training, validation, and testing phase. The live deployment of TIM-TOM will be released soon, integrating with the Metatrader5 trading platform. Developed using Python and leveraging the Tensorflow architecture, TIM-TOM showcases its advanced capabilities.

TIM-TOM Process:

(1) Prepare Data:

- Preprocess training and validation data for the agent, as well as deployment data for mt5. (Code complete) (Task complete)

(2) Train an initial state of TIM-TOM:

- Utilize a randomly selected sample of preprocessed historical EUR-USD pairs data at a randomly selected M15 bar. (Code complete) (Task complete)

(3a) Continue training the TIM-TOM state:

- Employ Transfer Learning techniques to update the agent's model states using randomly selected samples of preprocessed historical EUR-USD pairs data at randomly selected M15 bars. (Code complete) (Task in progress) (Note: Continuing to train the agent on randomly selected samples of preprocessed historical EUR-USD pairs data at randomly selected M15 bars.)

(3b) Periodically validate the TIM-TOM state:

- Ensure the agent updates correctly and make necessary parameter adjustments. Utilize optimization techniques to enable the agent to tune over time and reach optimal outputs. (Code complete) (Task in progress) (Note: Capturing validation data periodically as the TIM-TOM state trains.)

(4) Deployment of TIM-TOM:

- Incorporate the custom deep learning architecture and sub-agents into live market conditions using mt5 demo account, powered by an API script. Track relevant metrics for the agent's data consumption. (Code in progress) (Task in progress) (Note: An original version of the custom neural network architecture, used by TIM-TOM's various sub-agents, is being employed to test the agent's activity with mt5's platform and API instructions. We will provide a progress report on a single network agent named KBAI at 60-day intervals to assess its interaction with the markets. This data will be used to upgrade the necessary components of the code and hardware for optimized interaction between the agent and mt5 resources.)

(5) Live trading with real money using the TIM-TOM trading agent:

- Refer to step 4. Once this is complete and TIM-TOM demonstrates expected performance in real market conditions for 60 days, TIM-TOM will be officially launched.

Please note that while KBAI utilizes the same custom deep learning architecture as TIM-TOM, it serves as a dedicated Deep SARSA RL agent for testing agent parameters in live conditions using mt5's platform and API resources. KBAI's results during its live demo testing will contribute valuable data to optimize TIM-TOM's deployment resources. Monitoring KBAI's progress as it approaches the 60-day mark will provide significant insights for further enhancements and refinements.

Snippet examples of TIM-TOM's training: 

![signal-2023-06-19-225432_002](https://github.com/jkorn81/TIM-TOM/assets/47157865/733fb396-d83f-43f0-a1be-def4856d1a3a)

![signal-2023-06-19-225432_002](https://github.com/jkorn81/TIM-TOM/assets/47157865/f3397e29-e555-4cfc-bdc5-335592a3fa97)
