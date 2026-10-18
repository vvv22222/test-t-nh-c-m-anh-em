#include <iostream>
#include <string>
#include <thread>
#include <chrono>

using namespace std;

int main() {
    // Cấu hình hiển thị tiếng Việt (nếu trình duyệt hỗ trợ)
    cout << "\n========================================\n";
    cout << "   CHƯƠNG TRÌNH XÁC ĐỊNH ĐỘ TIN CẬY\n";
    cout << "========================================\n\n";

    string answer;
    
    cout << "Câu 1: Bạn có phải là co chó không? (Y/N): ";
    cin >> answer;

    if (answer == "Y" || answer == "y") {
        cout << "\n=> Chính xác !\n\n";
    } else {
        cout << "\n=> Sai rồi! Hệ thống buộc phải ép bạn nhận sự thật nàyyyyy...\n\n";
    }

    // Tạo hiệu ứng giả vờ đang hack/xử lý dữ liệu cho vui
    cout << "Đang kiểm";
    for (int i = 0; i < 3; i++) {
        this_thread::sleep_for(chrono::milliseconds(500));
        cout << ".";
        cout.flush();
    }
    
    cout << "\n\n----------------------------------------\n";
    cout << " KẾT QUẢ CUỐI CÙNG:\n";
    cout << " bạn là một cho chó\n";
    cout << "----------------------------------------\n";

    return 0;
}
