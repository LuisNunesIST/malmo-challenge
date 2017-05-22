###VIDEO###
https://vimeo.com/218450677

###FULL REPORT###
https://tinyurl.com/spartagusAI

To run our agent you have to run two instances of Minecraft (port 10000 and 10001 preferenciable). After that you have 2 choices:

1. Run the pig_chase_baseline.py python program (located in malmo-challenge/ai_challenge/pig_chase) if you want to see a automatic interaction of our agent with another of your choice:
	You can choose the agent by editing the line 69 of the file agent.py "return self._agents[X]", where X is the agent you want to execute:
		X=1: Focused Agent;
		X=2: Random Agent;
		X=3: Our Agent;

2. Run the pig_chase_human_vs_agent.py python program (located in malmo-challenge/ai_challenge/pig_chase) if you want to interact with our agent while controlling the colaborator agent (player 2);

Our implementation is the class HeuristicFocusedAgent (Line 529) in the file Agent.py. 

Our approach consists in a pratical reasoning agent, that decides the next action to take based on the current state of the environment and a set of heuristics defined by us. A meta-heuristic function receives all the heuristics and returns a probability to collaborate. A plan will then be created depending on the intention that was created.