# Python quiz game
import random

questions = (
    " What is earth's most abundant gas?",
    " How many bones are there in the human body?",
    " Which animal lays the largest egg?",
    " Who is the father of the atomic bomb?",
    " Which country has more lakes?",
    " What is the largest planet in the solar system?",
    " What is the chemical symbol for Gold?",
    " Which river is the longest river in the world?",
    " What is the largest ocean on the Earth?",
    " Which country gifted the statue of liberty to U.S?",
    " What is the currency of Japan?",
    " What is the tallest mountain in the world?",
    " What is the largest mammal in the world?",
    " Who wrote the play 'Romeo and Juliet'?",
    " What is the hardest natural substance in the world?"
)

options = (
    ("A) Oxygen", "B) Nitrogen", "C) Hydrogen", "D) Helium"),
    ("A) 207", "B) 205", "C) 206", "D) 201"),
    ("A) Elephant", "B) Ostrich", "C) Turtle", "D) Crocodile"),
    ("A) Newton", "B) Oppenheimer", "C) Tesla", "D) Graham Bell"),
    ("A) Australia", "B) America", "C) Canada", "D) Sri Lanka"),
    ("A) Saturn", "B) Jupiter", "C) Neptune", "D) Earth"),
    ("A) Gd", "B) Go", "C) Au", "D) Ag"),
    ("A) Amazon", "B) Nile", "C) Yangtze", "D) Mississippi"),
    ("A) Atlantic Ocean", "B) Indian Ocean", "C) Arctic Ocean", "D) Pacific Ocean"),
    ("A) United Kingdom", "B) Spain", "C) France", "D) Italy"),
    ("A) Won", "B) Yuan", "C) Yen", "D) Ringgit"),
    ("A) K2", "B) Kangchenjunga", "C) Mount Everest", "D) Lhotse"),
    ("A) African Elephant", "B) Blue Whale", "C) Giraffe", "D) Sperm Whale"),
    ("A) Charles Dickens", "B) William Shakespeare", "C) Jane Austen", "D) Oscar Wilde"),
    ("A) Quartz", "B) Diamond", "C) Titanium", "D) Granite")
)

answers = ("B", "C", "B", "B", "C", "B", "C", "B", "D", "C", "C", "C", "B", "B", "B")

# Pair each question with its options and answer, then shuffle the PAIRS (not each list separately)
quiz_data = list(zip(questions, options, answers))
random.shuffle(quiz_data)

guesses = []
score = 0

for question_num, (question, opts, correct_answer) in enumerate(quiz_data):
    print("---------------------")
    print(question)
    for option in opts:
        print(option)
    guess = (input("Enter(A ,B ,C ,D): ")).upper()
    guesses.append(guess)
    if guess == correct_answer:
        score += 1
        print("CORRECT!")
    else:
        print("INCORRECT!")
        print(f"{correct_answer} is the correct answer")

print("-----------------------")
print("--------RESULT---------")
print("-----------------------")

print("answers:", end=" ")
for _, _, correct_answer in quiz_data:
    print(correct_answer, end=" ")
print()

print("guesses:", end=" ")
for guess in guesses:
    print(guess, end=" ")
print()


score_percent = int(score / len(quiz_data) * 100)
print("---------------------------------")
print(f"Your score is: {score_percent}% ")
print("---------------------------------")
