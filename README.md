# learning_before_understanding.py

# sometimes i learn things before i really understand them.
# i copy commands.
# i follow tutorials.
# i run things and hope they work.
# sometimes they break.

class LearningProcess:
    def __init__(self):
        self.confused = True
        self.attempts = 0

    def try_again(self):
        self.attempts += 1
        if self.attempts > 3:
            self.confused = False

    def learn(self):
        while self.confused:
            self.try_again()
        return "now it makes sense."

if __name__ == "__main__":
    lp = LearningProcess()
    print(lp.learn())
