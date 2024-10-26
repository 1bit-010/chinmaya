chinmaya.1
this is my frist git Ripository
Author- chinmaya 
questions = [
    {
        "question": "What is the capital of France?",
        "options": ["A. Berlin", "B. Madrid", "C. Paris", "D. Lisbon"],
        "answer": "C"
    },
    {
        "question": "Which planet is known as the Red Planet?",
        "options": ["A. Earth", "B. Mars", "C. Jupiter", "D. Venus"],
        "answer": "B"
    },
    {
        "question": "Who wrote 'Hamlet'?",
        "options": ["A. Charles Dickens", "B. J.K. Rowling", "C. William Shakespeare", "D. Mark Twain"],
        "answer": "C"
    },
    {
        "question": "What is the largest mammal in the world?",
        "options": ["A. Elephant", "B. Blue Whale", "C. Giraffe", "D. Polar Bear"],
        "answer": "B"
    }
]


score = 0


for i, question in enumerate(questions):
    print(f"\nQuestion {i + 1}: {question['question']}")
    
    # Print the options
    for option in question['options']:
        print(option)
    
   
    answer = input("Enter your answer (A, B, C, or D): ").upper()
    
  
    if answer == question['answer']:
        print("Correct!")
        score += 1  # Increment score if correct
    else:
        print(f"Wrong! The correct answer was {question['answer']}.")


print(f"\nQuiz Over! Your final score is {score} out of {len(questions)}.")
