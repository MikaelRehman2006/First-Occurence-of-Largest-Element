# First-Occurence-of-Largest-Element
Finds the first occurrence of the largest element in a list

    int[] randList = {10, 20, 66, 20, 66, 87};
		
		int max = randList[0];
		int maxIndex = 0;
		for(int i = 0; i < randList.length; i++)
		{
		  if (randList[i] == max)
		  {
		    max = randList[i];
		    maxIndex = i;
		  } 
		}
		randList[maxIndex] = randList[randList.length - 1];
		randList[randList.length - 1] = max;

