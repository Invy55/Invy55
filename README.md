```python
from pyrogram import Client
import asyncio
from visitor import uid, name
from me import apiid, apihash

invy = Client("invy", apiid, apihash)

message = f"""
šš» Hi <i>{name}</>, Iām Marco (AKA @Invy55),
Iām a young boy <b>learning to code</>.
You can reach me at https://t.me/proporre or
just chec out <a href= "https://invy55.me">my website</>.
"""

async def main():
    await invy.start()
    await invy.send_message(uid, message)
    await invy.stop()

if __name__ == '__main__':
    asyncio.get_event_loop().run_until_complete(main())
```
