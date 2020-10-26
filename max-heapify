#include <iostream> 
  
using namespace std; 
void heapify(int arr[], int n, int i) 
{ 
    int largest = i; 
    int l = 2 * i + 1; 
    int r = 2 * i + 2; 
  
    if (l < n && arr[l] > arr[largest]) 
        largest = l; 
  
    if (r < n && arr[r] > arr[largest]) 
        largest = r; 
  
    if (largest != i) { 
        swap(arr[i], arr[largest]); 
  
        heapify(arr, n, largest); 
    } 
} 
  
void buildHeap(int arr[], int n) 
{ 
    int startIdx = (n / 2) - 1; 
  
    for (int i = startIdx; i >= 0; i--) { 
        heapify(arr, n, i); 
    } 
} 
  
void printHeap(int arr[], int n) 
{ 
    cout << "\nArray representation of Heap is:\n"; 
  
    for (int i = 0; i < n; ++i) 
        cout << arr[i] << " "; 
    cout << "\n"; 
} 
int main() 
{ 
    
    int n;
    cout<<"\nHow many elements you want to enter ? :";
    cin>>n;
    int arr[n];
    for (int i=0;i<n;i++)
    cin>>arr[i];
  	for (int i=0;i<n;i++)
    cout<<" "<<arr[i];
    int x = sizeof(arr) / sizeof(arr[0]); 
  
    buildHeap(arr, x); 
  
    printHeap(arr, x); 
    
    return 0; 
} 
