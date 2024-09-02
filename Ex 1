class mostWater {
  public int maxArea(int[] height) {
    int res = 0;
    int left = 0;
    int right = height.length - 1;

    while (left < right) {
      final int minHeight = Math.min(height[left], height[right]);
      res = Math.max(res, minHeight * (right - left));
      if (height[left] < height[right])
        ++left;
      else
        --right;
    }

    return res;
  }

  public static void main(String[] args) {
    mostWater sc = new mostWater();
    int[] height = {1, 8, 6, 2, 5, 4, 8, 3, 7}; 
    int result = sc.maxArea(height);
    System.out.println("Maximum area: " + result);
  }
}
