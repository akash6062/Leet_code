class Solution {
public:
    bool canVisitAllRooms(vector<vector<int>>& rooms) {
        unordered_set<int> visited;
        dfs(rooms, 0, visited);
        return visited.size() == rooms.size();
    }
    
    void dfs(const vector<vector<int>> & rooms,
             int cur, unordered_set<int> & visited) {
        visited.insert(cur);
        for (int neigh : rooms[cur])
            if (!visited.count(neigh))
                dfs(rooms, neigh, visited);
    }
};
