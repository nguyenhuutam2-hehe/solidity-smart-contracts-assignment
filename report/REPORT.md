## 01 Storage
- What it does : lưu và cập nhật một số uint256 trên blockchain
- Key concept : state variable, event, view function
- Tested : deploy(42), get() = 42, set(100) từ Account 2, get() = 100
- Ganache proof: screenshots/01_compile.png, 01_test1.png

## 02 Greeting
- What it does : lưu lời chào, chỉ owner được đổi, ai cũng đọc được
- Key concept : require() kiểm tra quyền, event, constructor gán owner
- Tested : greet(), setGreeting("GM Ganache") từ owner, setGreeting từ Account 2 -> revert "Not the owner", resetGreeting()
- Ganache proof: screenshots/02_compile.png, 02_test1.png, 02_test2.png

## 02 Greeting
- What it does : lưu lời chào, chỉ owner được đổi, ai cũng đọc được
- Key concept : require() kiểm tra quyền, event, constructor gán owner
- Tested : greet(), setGreeting("GM Ganache") từ owner, setGreeting từ Account 2 -> revert "Not the owner", resetGreeting()
- Ganache proof: screenshots/02_compile.png, 02_test1.png

## 03 Counter
- What it does : bộ đếm giới hạn trong [0, 100], có increment, decrement, reset
- Key concept : require() bảo vệ biên, constant, event
- Tested : decrement tại 0 -> revert "Count is zero", increment tới 100 -> revert "Max limit reached", reset
- Ganache proof: screenshots/03_compile.png
