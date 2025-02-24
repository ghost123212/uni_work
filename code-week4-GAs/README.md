# vacuum
Run the game using: __python3 game.py__

# you need to write this method
        # Select an individual from the population based on fitness values
        selected = random.sample(range(len(self.population)), k)  # Randomly sample k indices from the population
        best = selected[0]  # Start by assuming the first selected index is the best

        # Iterate through the selected indices to find the one with the lowest fitness value
        for index in selected:
            # If the fitness of the current individual is better (lower) than the current best, update best
            if self.fitnesses[index] < self.fitnesses[best]:
                best = index  # Update best to the current index if it has a better fitness

        # Return the individual from the population corresponding to the best fitness found
        return self.population[best]



