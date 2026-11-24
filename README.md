#include <stdio.h>
#define SIZE 10
#define EMPTY -1

int hashFunction(int key) {
  return key % SIZE;
}

void inser(int hashTable[], int key) {
 int index = hashFunction(key); 
int originalIndex = index;

 while (hashTable[index] != EMPTY) {
  index = (index +1)  % SIZE;

 if (index == originalIndex) { 
printf("Hash table is full ! Cannot insert %d\n", key)
return;
  }
}

int main() { 
int hashTable[SIZE];
int values[] = {23,45,12,34,67,89,90};
int n = sizeof(values) / sizeof(values[0]);

for (int i = 0; i < size; i++){
hashTable[i] = EMPTY
}

 for(int i = 0; i<n; i++){
   insert(hashTable, values[i]);
}

display(hashTable);

return 0;
}# Hash
