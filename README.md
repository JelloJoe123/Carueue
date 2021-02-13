# Carueue
#Where in the Queue is Carmen Sandiago?

class Queue:

  def __init__(self):
    self.data = []

  def enter(self, top):
    self.data.insert(0,top)
    pass

  def leave(self):
    return self.data.pop()

  def showQueue(self):
    return self.data


queue = Queue()
queue.enter('3')

if start == False:
  while next:

    question = input('Would you like to add or remove to the queue?\n')

    if question.lower() == 'yes':
      question1 = input('What would you like to do? Add or remove to your queue?\n')

      if question1.lower() == 'add':
        question2 = input('What would you like to add?\n')

        n = str(question2)

        queue.enter(n)
      elif question1.lower() == 'remove':
        queue.leave()
      else:
        print("Please enter 'add' or 'remove'.")

      question3 = input('Enter something to check if it is in the queue.\n')

      if question3 in queue.showQueue():
        print('This is in the queue. True')
      else:
        print('This is not in the queue. False')
    elif question.lower() == 'no':
      start = False
    else:
      print("Please enter 'yes' or 'no'.")
    print(queue.showQueue())
