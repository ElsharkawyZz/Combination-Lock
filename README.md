# Combination-Lock

#include <bits/stdc++.h>
#include <ctime>
using namespace std;

int main()
{
    ios_base::sync_with_stdio(0);
    cin.tie(0);
    cout.tie(0);
    int num;
    cin >> num;
    string sum1;
    string sum2;
    cin >> sum1 >> sum2;
    long long count = 0;
    for (int i = 0; i < num; i++)
    {
        count += min((abs(ssum1[i] - ssum2[i])), (10 - max(sum1[i] - '0', sum2[i] - '0') + min(sum1[i] - '0', sum2[i] - '0')));
    }
    cout << count << endl;
    return 0;
}
