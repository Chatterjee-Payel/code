# code
class Solution
{
    public:
    //Function to find the maximum occurring character in a string.
    char getMaxOccuringChar(string str)
    {
        // Your code here
         map<char,int>freq;
        int max=-1;
        char c;
        for(int i=0;i<str.size();i++)
        {
            freq[str[i]]++;
        }
      
        for(auto i:freq){
            if(i.second>max)
            {
                max=i.second;
                c=i.first;
            }
        }
        return c;
    }
};
