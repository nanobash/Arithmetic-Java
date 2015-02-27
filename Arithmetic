public class Arithmetic {

	public static int[] merge(int[] listA, int[] listB) {
		int[] merged = new int[listA.length + listB.length];
		int c = 0;

		for (int v: listA) {
			merged[c] = v;
			c++;
		}

		for (int v: listB) {
			merged[c] = v;
			c++;
		}

		selectionSortAsc(merged);

		return merged;
	}

	public static boolean isSortedAsc(int[] list) {
		boolean flag = true;
		int temp = list[0];

		for (int i = 1; i < list.length; i++) {
			if (temp > list[i]) {
				flag = false;
				break;
			}
			temp = list[i];
		}

		return flag;
	}

	public static boolean isSortedAsc(double[] list) {
		boolean flag = true;
		double temp = list[0];

		for (int i = 1; i < list.length; i++) {
			if (temp > list[i]) {
				flag = false;
				break;
			}
			temp = list[i];
		}

		return flag;
	}

	public static int[] unique(int[] list) {
		int[] t = new int[list.length];

		for (int i = 0; i < list.length; i++) {
			boolean flag = true;

			for (int j = 0; j < list.length; j++) {
				if (i == j) {
					continue;
				}

				if (list[i] == list[j]) {
					flag = false;
					break;
				}
			}
			
			if (flag) {
				t[i] = list[i];
			}
		}

		int c = 0, j = 0;

		for (int v: t)
			c += (v == 0) ? 0 : 1;

		int[] newList = new int[c];

		for (int i = 0; i < t.length; i++) {
			if (t[i] != 0) {
				newList[j] = t[i];
				j++;
			}
		}

		return newList;
	}

	public static double[] unique(double[] list) {
		double[] t = new double[list.length];
		
		for (int i = 0; i < list.length; i++) {
			boolean flag = true;
			
			for (int j = 0; j < list.length; j++) {
				if (i == j) {
					continue;
				}
				
				if (list[i] == list[j]) {
					flag = false;
					break;
				}
			}
			
			if (flag) {
				t[i] = list[i];
			}
		}
		
		int c = 0, j = 0;
		
		for (double v: t)
			c += (v == 0) ? 0 : 1;
		
		double[] newList = new double[c];
		
		for (int i = 0; i < t.length; i++) {
			if (t[i] != 0) {
				newList[j] = t[i];
				j++;
			}
		}
		
		return newList;
	}

	public static int[] duplicate(int[] list) {
		int[] t = new int[list.length];

		for (int i = 0; i < list.length; i++) {
			for (int j = i + 1; j < list.length; j++) {
				if (list[i] == list[j]) {
					t[i] = list[i];
				}
			}
		}

		return distinct(t);
	}

	public static double[] duplicate(double[] list) {
		double[] t = new double[list.length];

		for (int i = 0; i < list.length; i++) {
			for (int j = i + 1; j < list.length; j++) {
				if (list[i] == list[j]) {
					t[i] = list[i];
				}
			}
		}

		return distinct(t);
	}

	public static int[] distinct(int[] list) {
		for (int i = 0; i < list.length; i++) {
			for (int j = i + 1; j < list.length; j++) {
				if (list[i] == list[j]) {
					list[i] = 0;
				}
			}
		}

		int c = 0, i = 0;

		for (int v : list)
			c += (v == 0) ? 0 : 1;

		int[] newList = new int[c];

		for (int j = 0; j < list.length; j++) {
			if (list[j] != 0) {
				newList[i] = list[j];
				i++;
			}
		}

		return newList;
	}

	public static double[] distinct(double[] list) {
		for (int i = 0; i < list.length; i++) {
			for (int j = i + 1; j < list.length; j++) {
				if (list[i] == list[j]) {
					list[i] = 0;
				}
			}
		}

		int c = 0, i = 0;

		for (double v : list)
			c += (v == 0) ? 0 : 1;

		double[] newList = new double[c];

		for (int j = 0; j < list.length; j++) {
			if (list[j] != 0) {
				newList[i] = list[j];
				i++;
			}
		}

		return newList;
	}

	public static void insertionSortAsc(int[] list) {
		for (int i = 1; i < list.length; i++) {
			int currentValue = list[i];
			int j;

			for (j = i - 1; j >= 0 && list[j] > currentValue; j--) {
				list[j + 1] = list[j];
			}

			list[j + 1] = currentValue;
		}
	}

	public static void insertionSortAsc(double[] list) {
		for (int i = 1; i < list.length; i++) {
			double currentValue = list[i];
			int j;

			for (j = i - 1; j >= 0 && list[j] > currentValue; j--) {
				list[j + 1] = list[j];
			}

			list[j + 1] = currentValue;
		}
	}

	public static void insertionSortDesc(int[] list) {
		for (int i = 1; i < list.length; i++) {
			int currentValue = list[i];
			int j;

			for (j = i - 1; j >= 0 && list[j] < currentValue; j--) {
				list[j + 1] = list[j];
			}

			list[j + 1] = currentValue;
		}
	}

	public static void insertionSortDesc(double[] list) {
		for (int i = 1; i < list.length; i++) {
			double currentValue = list[i];
			int j;

			for (j = i - 1; j >= 0 && list[j] < currentValue; j--) {
				list[j + 1] = list[j];
			}

			list[j + 1] = currentValue;
		}
	}

	public static void selectionSortAsc(int[] list) {
		for (int i = 0; i < list.length - 1; i++) {
			int currentValue = list[i];
			int currentIndex = i;

			for (int j = i + 1; j < list.length; j++) {
				if (currentValue > list[j]) {
					currentValue = list[j];
					currentIndex = j;
				}
			}

			if (currentIndex != i) {
				list[currentIndex] = list[i];
				list[i] = currentValue;
			}
		}
	}

	public static void selectionSortAsc(double[] list) {
		for (int i = 0; i < list.length - 1; i++) {
			double currentValue = list[i];
			int currentIndex = i;

			for (int j = i + 1; j < list.length; j++) {
				if (currentValue > list[j]) {
					currentValue = list[j];
					currentIndex = j;
				}
			}

			if (currentIndex != i) {
				list[currentIndex] = list[i];
				list[i] = currentValue;
			}
		}
	}

	public static void selectionSortDesc(int[] list) {
		for (int i = 0; i < list.length - 1; i++) {
			int currentValue = list[i];
			int currentIndex = i;

			for (int j = i + 1; j < list.length; j++) {
				if (currentValue < list[j]) {
					currentValue = list[j];
					currentIndex = j;
				}
			}

			if (currentIndex != i) {
				list[currentIndex] = list[i];
				list[i] = currentValue;
			}
		}
	}

	public static void selectionSortDesc(double[] list) {
		for (int i = 0; i < list.length - 1; i++) {
			double currentValue = list[i];
			int currentIndex = i;

			for (int j = i + 1; j < list.length; j++) {
				if (currentValue < list[j]) {
					currentValue = list[j];
					currentIndex = j;
				}
			}

			if (currentIndex != i) {
				list[currentIndex] = list[i];
				list[i] = currentValue;
			}
		}
	}

	public static int linerSearch(int[] list, int value) {
		for (int i = 0; i < list.length; i++) {
			if (list[i] == value) {
				return i;
			}
		}

		return -1;
	}

	public static int linerSearch(double[] list, double value) {
		for (int i = 0; i < list.length; i++) {
			if (list[i] == value) {
				return i;
			}
		}

		return -1;
	}

	public static int binarySearch(int[] list, int value) {
		int low = 0, high = list.length - 1;

		while (high >= low) {
			int mid = (low + high) / 2;

			if (value < list[mid]) {
				high = mid - 1;
			} else if (value == list[mid]) {
				return mid;
			} else {
				low = mid + 1;
			}
		}

		return -1;
	}

	public static int binarySearch(double[] list, double value) {
		int low = 0, high = list.length - 1;

		while (high >= low) {
			int mid = (low + high) / 2;

			if (value < list[mid]) {
				high = mid - 1;
			} else if (value == list[mid]) {
				return mid;
			} else {
				low = mid + 1;
			}
		}

		return -1;
	}

	public static double estimatePI(int n) {
		double sum = 0;

		for (int i = 1; i < n; i++) {
			sum += (Math.pow(-1, (i + 1))) / (2 * i - 1);
		}

		sum *= 4;

		return sum;
	}

	public static boolean isPalindrome(int num) {
		return (num == reverse(num)) ? true : false;
	}

	public static boolean isPalindrome(String str) {
		return (str.equals(reverse(str))) ? true : false;
	}

	public static int[] reverse(int[] list) {
		for (int i = 0, j = (list.length - 1); i < (list.length / 2); i++, j--) {
			int temp = list[i];
			list[i] = list[j];
			list[j] = temp;
		}

		return list;
	}

	public static double[] reverse(double[] list) {
		for (int i = 0, j = (list.length - 1); i < (list.length / 2); i++, j--) {
			double temp = list[i];
			list[i] = list[j];
			list[j] = temp;
		}

		return list;
	}

	public static int reverse(int num) {
		String reverse = "0";

		while (num != 0) {
			reverse += num % 10;
			num /= 10;
		}

		return Integer.parseInt(reverse);
	}

	public static String reverse(String str) {
		String reverse = "";

		for (int i = (str.length() - 1); i >= 0; i--) {
			reverse += str.charAt(i);
		}

		return reverse;
	}

	public static int sumDigits(int num) {
		int sum = 0;

		while (num != 0) {
			sum += num % 10;
			num /= 10;
		}

		return sum;
	}

	public static int getPentagonalNumber(int n) {
		return n * (3 * n - 1) / 2;
	}

	public static boolean isPrime(int x) {
		boolean flag = true;

		for (int i = 2; i <= x / 2; i++) {
			if (x % i == 0) {
				flag = false;
				break;
			}
		}

		return flag;
	}

	public static int gcd(int x, int y) {
		int gcd = 1, z = 2;

		while (z <= x && z <= y) {
			if (x % z == 0 && y % z == 0) {
				gcd = z;
			}
			z++;
		}

		return gcd;
	}
}
