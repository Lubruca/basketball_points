# MIT License
# This program counts the point of one person or one team by counting triples, regular shots and free throws.
# Create by : Lucas Flores Fernández 
# Date : 16/01/2025


# Algorithm: Calculate total basketball points

def calculate_basketball_points(triples, regular_shots, free_throws):
    """
    Calculate the total points in a basketball game.

    Parameters:
    triples (int): Number of 3-point shots made.
    regular_shots (int): Number of 2-point shots made.
    free_throws (int): Number of 1-point free throws made.

    Returns:
    int: Total points scored.
    """
    # Each type of shot contributes to the total points
    total_points = (triples * 3) + (regular_shots * 2) + free_throws
    return total_points

# Example usage
if __name__ == "__main__":
    # Inputs
    triples = int(input("Enter the number of 3-point shots made: "))
    regular_shots = int(input("Enter the number of 2-point shots made: "))
    free_throws = int(input("Enter the number of free throws made: "))

    # Calculate total points
    total = calculate_basketball_points(triples, regular_shots, free_throws)

    # Output the result
    print(f"Total points scored: {total}")
