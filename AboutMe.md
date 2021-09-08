# REHAMAN NAGURU ABDUR

I am from Tirupathi, Andhra pradesh state, India. I worked as Data Analyst in Amazon Development center in chennai for 1.5 years. I'm fond of Music and Gardening. I love Travelling and exploring new places.

**[Click Here for my image](mypicture.jpg)**

***

### Famous Foods IN INDIA

From my experiences these are the famous foods in india and it is worth to pay such amount for the delicious taste. I suggest everyone to try these foods atleast once in their lifetime.

| Food/Drink | Location | Cost |
| ---| ---| ---: |
| Bawarchi Briyani | Hyderabad,India | 160 INR (2USD) |
| Fish Fry | chennai,India | 200INR (2.7 USD) |
| Qureshi Kabab | chandini chowk,Delhi | 70 INR (1USD) |
| Rabri Falooda | gaini, Old Delhi | 100 INR (1.5USD) |

***

### Quotes That Will Inspire you Everyday

> The most effective way to do it is to do it.  -*amelia earhart*

> Every pain gives a lesson and every lesson changes a person.  -*A. P. J. Abdul Kalam*

> Peace begins with a smile.  -*Mother Teresa*

***

### Let's Learn some coding.

> I have an array of string, which holds the list of strings. I want to figure out is there any duplicate entries in this list. Basically i have a list of users, and there should be no duplicate entries.

**[Click Here for Description Page](https://stackoverflow.com/questions/15356974/how-to-find-duplicate-string-from-an-array-of-string)**


~~~

vector<vector<int>> group_identical_strings(vector<string> const& s) {
    int n = s.size();
    vector<pair<long long, int>> hashes(n);
    for (int i = 0; i < n; i++)
        hashes[i] = {compute_hash(s[i]), i};

    sort(hashes.begin(), hashes.end());

    vector<vector<int>> groups;
    for (int i = 0; i < n; i++) {
        if (i == 0 || hashes[i].first != hashes[i-1].first)
            groups.emplace_back();
        groups.back().push_back(hashes[i].second);
    }
    return groups;
}

~~~

Code Source Page <https://cp-algorithms.com/string/string-hashing.html#toc-tgt-2>
