import random

class Key:

    def __init__ (self, key=''):
        if key == '':
            self.key = self.generate()
    
    def generate(self):
        key = ''
        chunk = ''
        check_digit_count = 0
        alphabet = 'abcdefghijklmonpqrstuvwxyz1234567890'
        while len(key) < 25:
            char = random.choice(alphabet)
            key += char
            chunk += char
            if len(chunk) == 4:
                key += '-'
                chunk = ''
            Key = key[:-1]
        if Key(key).verify():
            return key
        else:
            key = ''
    print(Key)
"""
    def verify(self):
        score = 0
        check_digit = self.key[0]
        check_digit_count = 0
        chunks = self.key.split('-')
        for chunk in chunks:
            if len(chunk) !=4:
                return False
            for char in chunk:
                if char == check_digit:
                    check_digit_count += 1
                score += ord(char)
        if score == 1772 and check_digit_count == 3:
            return True
        return False
    def __str__(self):
        valid = 'Invalid key'
        if self.verify():                
            valid = 'Valid key'
            return self.key.upper() + ':' + valid
"""

    


