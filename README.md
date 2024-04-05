# arrays
using System;

namespace merge_arrays {
  class Program {
    static void Main(string[] args) {
      int[] arr1 = { 1, 2, 3 };
      int[] arr2 = { 4, 5, 6 };
      int[] arr3 = new int[arr1.Length + arr2.Length];
      Array.Copy(arr1, arr3, arr1.Length);
      Array.Copy(arr2, 0, arr3, arr1.Length, arr2.Length);
      foreach (var e in arr3) {
        Console.WriteLine(e);
      }
    }
  }
}
