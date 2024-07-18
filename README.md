import time
def calculate_wpm(text, time_taken):
 words = text.split()
word_count = len(words) minutes = time_taken / 60  # Convert time_taken to 
minuteswpm = word_count / minutes if minutes > 0 else 0  return wpm
def typing_speed_test(text):
print("Type the following text:")
  print(text)
    
 input("Press Enter when ready to start...")
    
  start_time = time.time()
  user_input = input("Start typing here:\n")
  end_time = time.time()
    
 time_taken = end_time - start_time
    
wpm = calculate_wpm(text, time_taken)
print(f"\nYour typing speed: {wpm:.2f} WPM")

# Example text for typing test
text_to_type = "The quick brown fox jumps over the lazy dog."

typing_speed_test(text_to_type)



 
