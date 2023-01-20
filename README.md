# Carpet-Cleaning
#include <iostream>

int main(){
    std::cout << "Hello, welcome to Frank's Carpet Cleaning Service \n\n";
    
    std::cout << "How many small rooms would you like cleaned? ";
    int num_small_rooms(0);
    std::cin >> num_small_rooms;
    
    std::cout << "How many large rooms would you like cleaned? ";
    int num_large_rooms(0);
    std::cin >> num_large_rooms;
    
    std::cout << "Number of small rooms: " << num_small_rooms << "\n";
    std::cout << "Number of large rooms: " << num_large_rooms << "\n";
    
    std::cout << "Price per small room: $25 \n";
    std::cout << "Price per large room: $35 \n";
    
    
    const int price_small(25);
    const int price_large(35);
    const double tax(6.6);
    int cost((num_large_rooms * price_large) + (num_small_rooms*price_small));
    double pre_tax_total((num_large_rooms * price_large) + (num_small_rooms*price_small));
    
    
    std::cout << "Cost: $"<< cost << "\n";
    std::cout << "Tax: $"<< tax << "\n";
    
    std::cout << "--------------------------------\n";
    
    std::cout << "Total Estimate: $" << pre_tax_total + tax << "\n";
    std::cout <<"This estimate is valid for 30 days." << "\n";
}
