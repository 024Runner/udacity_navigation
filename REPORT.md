<h1>Abstract</h1>
<h2>Deep Q-Networks</h2>

Deep neural networks act as function approximators.  Specifically, Deep Q-Networks are multi-layered neural networks
that for a given state output a vector of action values with the max value indicating the action to take.  Reward changes are fed back as the reinforcement signal at each time step.  It stands to reason that, in the beginning, actions are vastly innapropriate because the neural network is initialized with random values.  Hence, it also stands to reason that, in time, actions become more appropriate as the neural network learns to associate states and state sequences with actions.

<h2>Input State Space</h2>

Even though input state spaces remain technically discrete, they can be very large and difficult to process.  To that end, in order to simplify the problem and optimize the solution, it may be necessary to scale down the input state space in order to leverage optimized neural network operations on GPUs.

<h2>Action Vector Output</h2>

Deep Q-Networks are designed to produce a Q-value for every possible action in a single forward pass.  This avoids having to run the neural network individually for every action.
