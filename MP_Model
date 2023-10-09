class MPNeuron:
    def __init__(self, weights, threshold):
        self.weights = weights
        self.threshold = threshold

    def activate(self, inputs):
        weighted_sum = sum(w * x for w, x in zip(self.weights, inputs))
        if weighted_sum >= self.threshold:
            return 1
        else:
            return 0

# Implement the AND gate
def AND_gate(inputs):
    weights = [1, 1]  # Weights for the two inputs
    threshold = 2    # Threshold for the AND gate
    and_neuron = MPNeuron(weights, threshold)
    return and_neuron.activate(inputs)

# Implement the OR gate
def OR_gate(inputs):
    weights = [1, 1]  # Weights for the two inputs
    threshold = 1    # Threshold for the OR gate
    or_neuron = MPNeuron(weights, threshold)
    return or_neuron.activate(inputs)

# Implement the NOT gate
def NOT_gate(input):
    weight = -1      # Weight for the input
    threshold = 0    # Threshold for the NOT gate
    not_neuron = MPNeuron([weight], threshold)
    return not_neuron.activate([input])

# Test the gates
print("AND Gate:")
print(AND_gate([0, 0]))  # Should output 0
print(AND_gate([0, 1]))  # Should output 0
print(AND_gate([1, 0]))  # Should output 0
print(AND_gate([1, 1]))  # Should output 1

print("\nOR Gate:")
print(OR_gate([0, 0]))   # Should output 0
print(OR_gate([0, 1]))   # Should output 1
print(OR_gate([1, 0]))   # Should output 1
print(OR_gate([1, 1]))   # Should output 1

print("\nNOT Gate:")
print(NOT_gate(0))  # Should output 1
print(NOT_gate(1))  # Should output 0
