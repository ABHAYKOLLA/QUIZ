# QUIZ
quiz = [
    {
        "question": "What is the capital city of India?",
        "options": ["A. Mumbai", "B. New Delhi", "C. Bengaluru", "D. Kolkata"],
        "answer": "B"
    },
    {
        "question": "Who was the first Prime Minister of independent India?",
        "options": ["A. Mahatma Gandhi", "B. Sardar Patel", "C. Jawaharlal Nehru", "D. Subhas Chandra Bose"],
        "answer": "C"
    },
    {
        "question": "Which Indian state is known as the 'Land of Five Rivers'?",
        "options": ["A. Punjab", "B. Haryana", "C. Gujarat", "D. Bihar"],
        "answer": "A"
    },
    {
        "question": "In which year did India gain independence from British rule?",
        "options": ["A. 1945", "B. 1947", "C. 1950", "D. 1952"],
        "answer": "B"
    },
    {
        "question": "Which Indian festival is known as the 'Festival of Lights'?",
        "options": ["A. Holi", "B. Diwali", "C. Dussehra", "D. Raksha Bandhan"],
        "answer": "B"
    },
    {
        "question": "Who wrote the Indian national anthem 'Jana Gana Mana'?",
        "options": ["A. Rabindranath Tagore", "B. Bankim Chandra Chatterjee", "C. Sarojini Naidu", "D. Lata Mangeshkar"],
        "answer": "A"
    },
    {
        "question": "What is the national animal of India?",
        "options": ["A. Elephant", "B. Lion", "C. Tiger", "D. Leopard"],
        "answer": "C"
    },
    {
        "question": "Which river is considered the holiest in India?",
        "options": ["A. Yamuna", "B. Narmada", "C. Godavari", "D. Ganga"],
        "answer": "D"
    }
]

def run_quiz(questions):
    score = 0
    print("\n🇮🇳 Welcome to the Quiz Game! 🇮🇳\n")

    for index, q in enumerate(questions):
        print(f"Q{index + 1}: {q['question']}")
        for option in q['options']:
            print(option)
        answer = input("Your answer (A/B/C/D): ").strip().upper()

        if answer == q['answer']:
            print("✅ Correct!\n")
            score += 1
        else:
            print(f"❌ Wrong! The correct answer was {q['answer']}.\n")

    print(f" Quiz Complete! Your final score is {score}/{len(questions)}.\n")
    
run_quiz(quiz)
